# Hesap-Makinesi
Hesap Makinesini switch-case kullanarak oluşturma

package Giris;
import java.util.Scanner;

public class hesap_makinesi {
    public static void main(String[] args){
        Scanner input =  new Scanner(System.in);

        System.out.print("ilk sayıyı girin: ");
        double ilk= input.nextDouble();
        System.out.print("ikinci sayıyı girin: ");
        double ikinci= input.nextDouble();

        System.out.println("Toplama: 1\nÇıkarma: 2\nÇarpma: 3\nBölme:4 ");
        System.out.println("Seçiminizi yapınız: ");
        int select=input.nextInt();

        switch(select){
            case 1:
                System.out.println(ilk + ikinci);
                System.out.println("Toplama sonucu: " +(ilk+ikinci));
                break;
            case 2:
                System.out.println("Çıkarma sonucu: " +(ilk-ikinci));
                break;
            case 3:
                System.out.println("Çarpma sonucu: " +(ilk*ikinci));
                break;
            case 4:
                if(ikinci!=0)
                    System.out.println("Bölme sonucu: " +(ilk/ikinci));
                else
                    System.out.println("Bir sayı sıfıra bölünemez. Sonuç tanımsız.");
                break;
            default:
                System.out.println("Geçersiz seçim.");

        }
    }
}
