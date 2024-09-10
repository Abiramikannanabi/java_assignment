public class WordEncryption {

    public static String encryptString(String input1, int input2) {
        StringBuilder encryptedWord = new StringBuilder();

        for (char ch : input1.toCharArray()) {
            if (Character.isLetter(ch)) {
                int charValue = Character.isLowerCase(ch) ? ch - 'a' : ch - 'A';
                int encryptedValue = (charValue + input2) % 26;
                char encryptedChar = (char) ((Character.isLowerCase(ch) ? 'a' : 'A') + encryptedValue);
                if (Character.isLowerCase(ch)) {
                    encryptedChar = Character.toUpperCase(encryptedChar);
                } else {
                    encryptedChar = Character.toLowerCase(encryptedChar);
                }

                encryptedWord.append(encryptedChar);
            } else {
                encryptedWord.append(ch);
            }
        }

        return encryptedWord.toString();
    }

    public static void main(String[] args) {
        String input1 = "Wipro Tech";
        int input2 = 20;
        String encrypted = encryptString(input1, input2);
        System.out.println("Encrypted words: " + encrypted);
    }
}
