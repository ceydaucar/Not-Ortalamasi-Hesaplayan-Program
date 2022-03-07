# NotOrtalamasiHesaplayanProgram
Patika.dev > Java101 > Temel Kavramlar ve Değişkenler > Pratik1 - Not Ortalaması Hesaplayan Program

## Java ile Matematik, Fizik, Kimya, Türkçe, Tarih, Müzik derslerinin sınav puanlarını kullanıcıdan alan ve ortalamalarını hesaplayıp ekrana bastırılan programı yazın. 
*Aynı program içerisinde koşullu ifadeler kullanılarak, eğer kullanıcının ortalaması 60'dan büyük ise ekrana "Sınıfı Geçti" , küçük ise "Sınıfta Kaldı" yazsın. * 
*Not : If ve Else kullanılmayacak.

	import java.util.*;
	
	public class pratik1 {
	
		public static void main(String[] args) {
			// Yeni bir tarayıcı(scanner) oluştur.
			Scanner sc = new Scanner(System.in);
		
			// Kullanıcıdan  Matematik, Fizik, Kimya, Türkçe, Tarih, Müzik derslerinin sınav puanlarını al.
			System.out.println("Matematik puanı: ");
			int matematik = sc.nextInt();
		
			System.out.println("Fizik puanı: ");
			int fizik = sc.nextInt();
		
			System.out.println("Kimya puanı: ");
			int kimya = sc.nextInt();
		
			System.out.println("Türkçe puanı: ");
			int turkce = sc.nextInt();
		
			System.out.println("Tarih puanı: ");
			int tarih = sc.nextInt();
		
			System.out.println("Müzik puanı: ");
			int muzik = sc.nextInt();
		
			// Puanları topla ve ders sayısına böl.
		
			int ortalama = (matematik + fizik + kimya + turkce + tarih + muzik) / 6;
		
			// Sınıfı geçip geçemediğini göster.
			System.out.println((ortalama > 60) ? "Sınıfı geçti" : "Sınıfta kaldı");
		
		}
	}
