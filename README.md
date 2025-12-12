# Sistem ve Ağ Bilgisi Tarayıcısı

Information Gathering, Footprinting

Bu script, çalıştırıldığı bilgisayarın temel özelliklerini analiz eder ve raporlar. Bir saldırganın veya sistem yöneticisinin, o makine hakkında ilk bakışta neleri görebileceğini simüle eder.

Tespit Ettiği Bilgiler:
- İşletim Sistemi Türü ve Sürümü (Windows/Linux vb.)
- İşlemci Mimarisi ve Bilgisayar Adı
- Yerel IP Adresi (LAN - Modemden alınan IP)
- Dış IP Adresi (WAN - İnternete çıkış IP'si)

Kullanılan Yöntem
Python'un standart "platform" ve "socket" kütüphanelerini kullanarak donanım ve ağ bilgilerini çektim. Dış IP adresini bulmak için ise "ipify" API servisine Python üzerinden bir HTTP isteği gönderdim. Bu sayede program, internete çıkış kimliğini de tespit edebiliyor.

Gereksinimler
Kodun çalışması için "requests" kütüphanesinin yüklü olması gerekir.
Kurulum: pip install requests

Nasıl Çalıştırılır?
Terminalde şu komutu yazmanız yeterlidir:
python scanner.py

Not
EĞİTİM AMAÇLIDIR.

Emircan Bingöl 
