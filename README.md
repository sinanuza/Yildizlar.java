# Yildizlar.java
www.patika.dev Yildizlarla Sekil olusturma



        import java.util.Scanner;

        public class yıldızlarla_ucgen {
        public static void main(String[] args) {
        int s, k, n;
        int yildiz = 1;
        System.out.println("Lutfen basamak sayisini girin:");
        Scanner input = new Scanner(System.in);
        n = input.nextInt();
        int bosluk = n - 1;
        for (k = 0; k < n; k++) {
            for (s = 0; s < bosluk; s++) {
                System.out.print(" ");
            }
            for (s = 0; s < yildiz; s++) {
                System.out.print("*");
            }
            System.out.println();
            bosluk--;
            yildiz += 2;
        }
        yildiz-=4;
        bosluk =1;
        for (k = 0; k < n; k++) {
            for (s = 0; s < bosluk; s++) {
                System.out.print(" ");
            }
            for (s = 0; s < yildiz; s++) {
                System.out.print("*");
            }
            System.out.println();
            bosluk++;
            yildiz -= 2;
        }
    }
}
