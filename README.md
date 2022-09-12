# Kdv_Hesap
Kdv_Hesap



import  java.util.Scanner;

public class kdv_tutari {
    public static void main(String[] args) {

        double tutar,kdvoran,kdvtutar,kdvlitutar;

        Scanner input= new Scanner(System.in);

        System.out.print("Ucret tutarı gırınız : ");
        tutar=input.nextDouble();


        if (tutar>=0 && tutar<=1000){
            kdvoran=0.18;
            kdvtutar=tutar*kdvoran;
            kdvlitutar=tutar+kdvtutar;

            System.out.println("Kdvsiz tutar : "+tutar);
            System.out.println("Kdv Oranı : "+kdvoran);
            System.out.println("Kdv tutar : "+kdvtutar);
            System.out.println("Kdvli tutar : "+kdvlitutar);

        }
        else {
            kdvoran=8;

            kdvtutar=tutar*kdvoran;
            kdvlitutar=tutar+kdvtutar;
            System.out.println("Kdvsiz tutar : "+tutar);
            System.out.println("Kdv Oranı : "+kdvoran);
            System.out.println("Kdv tutar : "+kdvtutar);
            System.out.println("Kdvli tutar : "+kdvlitutar);

        }





    }
}
