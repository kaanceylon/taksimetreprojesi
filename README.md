# taksimetreprojesi
Java ile gidilen mesafeye (KM) göre taksimetre tutarını ekrana yazdıran programı yazın.
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    int km;
    double perkm = 2.20, total, startPrice = 10;

    Scanner input = new Scanner(System.in);
    System.out.print("Taksimetre tutarını giriniz :");
    km = input.nextInt();

    total = km * perkm;
    total += startPrice;

    total = (total < 20 ) ? 20 : total;

    System.out.print("Toplam tutar : " + total );


    }
}
