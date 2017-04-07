import java.util.Scanner;
public class Fibonacci {
    public static void main(String[]args) {
		long a=0;
        Scanner show = new Scanner(System.in);
        System.out.print("Masukan Jumlah Deret Fibonacci : ");
        int n = show.nextInt();
        long fib[] = new long[n];
         
        fib[0] = 0;
        fib[1] = 1;
         
        for(int i = 2; i < n; i++) {
            fib[i] = fib[i-1] + fib[i-2];
        }
         
        for (int i = 1; i < n; i++) {
            System.out.print(fib[i] +  " ");
			a=a + fib[i];
        }
		System.out.println("\njumlah : "+a);
    }
 
}
