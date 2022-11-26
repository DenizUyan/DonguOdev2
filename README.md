import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.print("Bir Sayi Giriniz:");
        int a = input.nextInt();
        int toplam = 0;

        for(int i=1; i<a; i++){
            if(a%i == 0){
                toplam  = toplam + i;
            }
        }

        if(a == toplam){
            System.out.println(a+ " Mükemmel Sayidir");
        }
        else {
            System.out.println(a+ " Mükemmel Sayi Değildir");
        }

    }
}
