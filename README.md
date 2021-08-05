import java.util.Scanner;
 class Fibbonacci {
  public static void main(String[] args) {

    int n, firstTerm = 0, secondTerm = 1;
    System.out.println("Enter the number:");
     
     Scanner input = new Scanner(System.in);
     n = input.nextInt();
    System.out.println("Fibonacci Series till " + n + " terms:");

    for (int i = 1; i <= n; ++i) {
      System.out.print(firstTerm + ", ");
      
      int nextTerm = firstTerm + secondTerm;
      firstTerm = secondTerm;
      secondTerm = nextTerm;
    }
  }
}
