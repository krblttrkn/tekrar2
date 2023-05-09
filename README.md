# KDV Tutarı Hesaplayan Program
* Java ile kullanıcıdan alınan para değerinin KDV'li fiyatını ve KDV tutarını hesaplayıp ekrana bastıran programı yazın.
* (Not : KDV tutarını %18 olarak alın.)
* KDV'siz Fiyat = 10
* KDV'li Fiyat = 11.8
* KDV Tutarı = 1.8
# Ödev
* Eğer girilen tutar 0 ve 1000 TL arasında ise KDV oranı %18 , tutar 1000 TL'den büyük ise KDV oranını %8 olarak KDV tutarı hesaplayan program yazınız.

```
import java.util.Scanner;

public class Kdv {
    public static void main(String[] args){

        double tutar ,kdv,kdvTutari,kdvliTutar ;
        Scanner inp = new Scanner(System.in);
        System.out.print("Ücret Tutarını Giriniz : ");
        tutar = inp.nextDouble();

        boolean kdvOrani = (0<tutar)&&(tutar<1000);
        kdv = kdvOrani ? 0.18 : 0.08;

        kdvTutari=tutar*kdv;
        kdvliTutar=tutar+kdvTutari;

        System.out.println("KDV'siz Tutar : "+tutar);
        System.out.println("KDV Oranı : "+kdv);
        System.out.println("KDV Tutarı : "+kdvTutari);
        System.out.println("KDV'li Tutar : "+kdvliTutar);
    }
}
```
# Patika Linkim
<a href="https://academy.patika.dev/profile">Patika Profilim</a>