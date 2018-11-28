class StringDuplication {
    public static void main(String[ ] args) {
        String checkString = "Afterthought";
        char[] chars = checkString.toCharArray();
        System.out.println("Length" +chars.length);
        Map<Character, Integer> theString = new Hashmap<Character, Integer>();
        for (char duplicate: chars) {
            if (theString.containsKey(duplicate)) {
                theString.put(duplicate, theString.getValue(duplicate) + 1);
            }
            else {
                theString.put(duplicate, 1);
            }
        }
        
        System.out.println("The duplicate characters: " +theString);
    }
}

