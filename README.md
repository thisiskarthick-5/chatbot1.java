# chatbot1.java

    import java.util.Scanner;
    
    class main{
        public static void main(String[] args) {
            Scanner scanner = new Scanner(System.in);
            String userInput = "";
    
            System.out.println("Hello! I'm a simple chatbot. Type 'exit' to end the conversation.");
            
            while (true) {
                System.out.print("You: ");
                userInput = scanner.nextLine().toLowerCase(); // Convert input to lowercase
    
                if (userInput.equals("exit")) {
                    System.out.println("Chatbot: Goodbye!");
                    break;
                } else if (userInput.contains("hello")) {
                    System.out.println("Chatbot: Hi there!");
                } else if (userInput.contains("how are you")) {
                    System.out.println("Chatbot: I'm just a bunch of code, but I'm doing great! How about you?");
                } else if (userInput.contains("time")) {
                    System.out.println("Chatbot: I don't have a watch, but you can check your system clock!");
                } else if (userInput.contains("name")) {
                    System.out.println("Chatbot: I'm your friendly Java chatbot created by 'karthick' . What's your name?");
                } else {
                    System.out.println("Chatbot: Sorry, I don't understand that. Can you try asking something else?");
                }
            }
            
            scanner.close();
        }
    }
