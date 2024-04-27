# cinZodyag-
cinZodyagı hesaplama
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Kullanıcıdan doğum yılını al
        System.out.print("Doğum yılınızı girin: ");
        int dogumYili = scanner.nextInt();

        int kalan = dogumYili % 12;

        // Kalana göre Çin Zodyağı sembolü belirle
        String cinZodyagiSembolu = "";
        switch (kalan) {
            case 0:
                cinZodyagiSembolu = "Maymun";
                break;
            case 1:
                cinZodyagiSembolu = "Horoz";
                break;
            case 2:
                cinZodyagiSembolu = "Köpek";
                break;
            case 3:
                cinZodyagiSembolu = "Domuz";
                break;
            case 4:
                cinZodyagiSembolu = "Fare";
                break;
            case 5:
                cinZodyagiSembolu = "Öküz";
                break;
            case 6:
                cinZodyagiSembolu = "Kaplan";
                break;
            case 7:
                cinZodyagiSembolu = "Tavşan";
                break;
            case 8:
                cinZodyagiSembolu = "Ejderha";
                break;
            case 9:
                cinZodyagiSembolu = "Yılan";
                break;
            case 10:
                cinZodyagiSembolu = "At";
                break;
            case 11:
                cinZodyagiSembolu = "Koyun";
                break;
            default:
                System.out.println("Geçersiz doğum yılı!");
                return;
        }

        System.out.println("Çin Zodyağı sembolünüz: " + cinZodyagiSembolu);

        scanner.close();
    }
}
