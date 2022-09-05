# kdvHesaplamaProgram-

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        double fiyat,kdvF,kdv,kdvT ;
        
        //scanner tanımlanır çünkü kullanıcıdan değer istenir
        
        Scanner inp = new Scanner(System.in);
        
        //kullanıcıdan alınacak değer
        
        System.out.println("Kdv tutarı hesaplanacak değeri giriniz: ");
        
        fiyat= inp.nextDouble();
        
        //if else kullanılmadan kdv tutarı seçme
        
        kdv = fiyat < 1000 ? 0.18 : 0.08;
        
        kdvT=kdv*fiyat;
        
        kdvF=fiyat+(fiyat*kdv);
        
        //istenen çıktılar
        
        System.out.println("Hesaplanmasını İstediğiniz tutar: "+fiyat);
        
        System.out.println("Uygulanan Kdv Oranı: "+kdv);
        
        System.out.println("Kdv tutarı: "+kdvT);
        
        System.out.println("Kdv'li Fiyatı: "+kdvF);
    
    }

}