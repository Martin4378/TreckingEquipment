# TreckingEquipment
import java.util.Scanner;

public class P01_TreckingEquipment {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        int numberAlpinists = Integer.parseInt(scanner.nextLine());
        int numberKarabiners = Integer.parseInt(scanner.nextLine());
        int numberRopes = Integer.parseInt(scanner.nextLine());
        int numberPickels = Integer.parseInt(scanner.nextLine());

        double karabinerPrice = 36;
        double ropePrice = 3.60;
        double pickelPrice = 19.80;

        double equipmentSum = ((numberKarabiners * karabinerPrice) +
                (numberRopes * ropePrice) +  (numberPickels * pickelPrice));
        double totalSum = numberAlpinists * equipmentSum;
        double sumWithVAT = totalSum + (totalSum * 0.2);

        System.out.printf("%.2f\n",sumWithVAT);;
    }

}
