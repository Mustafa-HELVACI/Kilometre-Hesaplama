# Kilometre-Hesaplama
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        int km;
        // Kilometrre başı 2,20 TL, Taksimetre açılış ücreti 10TL.
        double perKm = 2.20, total, startPrice = 10;

        Scanner input = new Scanner(System.in);
        System.out.print("Mesafeyi KM cinsinden Giriniz :");
        km = input.nextInt();

        total = (km * perKm);
        total += startPrice;
        
        //Minimum ödenecek tutar 20 TL'dir. 20 TL altında ki ücretlerde yine 20 TL alınacaktır.
        total = (total < 20) ? 20 : total;
        System.out.println("Toplam Tutar : " + total);

    }
}
