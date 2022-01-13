# Tar Komutu Görsel Arayüzü

Linux Araçları ve Kabuk Programlama için yapılmış bir projedir.

## Proje
tar komutunun bazı parametreleri için zenity ile görsel bir arayüz oluşturulmuştur.
Dosya sıkıştırma ve ayıklama işlemleri yapılabilmektedir.

# Teknolojiler
- Bash Script
- Zenity

# Kurulum
## Github üzerinden indirmek

1) Repository sayfasındaki Code -> Download Zip kısmından zipi indirin.
2) Zipten çıkarın.
3) Zipten çıkarılmış klasorde terminali açın.
4) Terminalde "bash DosyaIslemleri.sh" komutunu çalıştırın.

## Git Üzerinden İndirmek ve Calistirmak
  Terminale aşağıdaki komutları sırasıyla girin.
- git clone https://github.com/keremersu35/TarWithZenity.git
- cd TarWithZenity
- bash DosyaIslemleri.sh

# Ekran Görüntüleri

## Ana Ekran
<img src="images/anaekran.png" >

- İlk olarak wget komutunu hangi parametre ile calistirmak istediginizi sectiginiz bir secim ekranı geliyor. Buradan istediginiz durumu seçip OK'a basarak devam ediyoruz.

## Devam/Cikis Yap
<img src="images/devam.png" >

- Daha sonrasında kullanıcıya devam edip etmek istemediği sorulur eğer devam seçeneği seçilirse kullanıcı yine seçim ekranına yönlendirilir.


## -i Parametresi
<img src="images/iparametresi.png" > <img src="images/linkler.png" >

- -i parametresi seçildiğinde ise kullanıcıdan bir dosya seçmesi istenir. 
- -i parametresinde kullanılmak için oluşturulan linkler.txt isimli dosya. Bu dosya file selection ile seçildikten sonra bütün linkler indirilir(Aynı dosya dizinine). Ve sonrasında kullanıcıya info ekranı gösterilir.

## -O Parametresi
<img src="images/oparametresi.png" > <img src="images/yeniisim.png" >

- -O parametresi girilen linkteki dosyayı farklı bir isimle kaydetmeye yarar. Kullanıcıdan bir link istendikten sonrasında kaydedileceği isimde istenir. Dosya yeni ismiyle aynı dizine indirilir.

## -P Parametresi
<img src="images/pparametre.png" > <img src="images/yenidizin.png" >

- -P parametresi girilen linkteki dosyayı farklı bir dizine kaydetmeye yarar. Kullanıcıdan bir link istendikten sonrasında kaydedileceği yeni dizinde istenir. Secil yapildiktan sonra dosya yeni dizine indirilir.

## -r -A Parametresi
<img src="images/raparametresi.png" > <img src="images/tur.png" >

- -r -A parametresi girilen linkteki sadece istenilen uzantili dosyaları indiren bir komuttur. Kullanıcıdan bir link istendikten sonrasında filtrelemek istedikleri uzantı sorulur sonrasında ise sadece istenen uzantidaki veriler indirilir.

## -b Parametresi/ --no-check-certificate Parametresi
<img src="images/bparametresi.png" > <img src="images/nocheck.png" >

- -b parametresi girilen linkteki dosyayı arka planda indirmeye yarar. 
- --no-check-certificate Geçersiz bir SSL sertifikasına sahip bir ana bilgisayardan HTTPS üzerinden bir dosya indirmeye yarar

<img src="images/basarisiz.png" >

- Gerekli alanlardan boş bırakılan olursa kullanıcıya warning ekranı gösterilir.
