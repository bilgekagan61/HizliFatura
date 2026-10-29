# Önceki aşamalar

29 Ekim 2026 tarihinde önceki konuşmalar incelenerek hazırlanmıştır. Yeni proje sıfırdan başlayacak; aşağıdakiler önceki çalışmanın hafızasıdır. Yeni projenin kapsamı, teknolojileri ve işleyişi henüz seçilmedi.

## Amaç ve ekip

Önceki çalışmada “HızlıFatura Akıllı Toplu e-Fatura ve e-Arşiv Yönetim Sistemi” adı kullanılmıştı. Amaç, çok sayıda fatura bilgisini hızlıca alıp kontrol ederek doğru firma için hazırlamaktı.

Ekip Bilge Kağan KALDIRIM ve Elif KARA olarak belirtilmiş; okul belgelerinde Bilge grup lideri seçilmişti. Proje iki kişiyle geliştirilecek. GitHub kullanıcı adları üzerinden erişim ayrıca düzenlenir.

## Daha önce yapılanlar

- Ham metinden toplu kayıt ayrıştırma, önizleme ve düzenleme üzerinde çalışılmıştı.
- Google Sheets bağlantısı ve tablo hücrelerine kopyala/yapıştır akışı geliştirilmişti.
- Kaynak tablonun 18 sütunundan gerekli 10 alanın alınması istenmişti: zaman damgası, plaka, şehir, istasyon/ilçe, ödeme yapanın adı, soyadı, telefon, TC/VKN, tutar ve satış kanalı.
- Seçilen günün `Zaman damgası` değerine göre filtrelenmesi; başka tarihli satırların alınmaması ve kaynak Sheet'in değiştirilmemesi kararlaştırılmıştı.
- Satış kanalından İKRADOR/TÜREV firma ayrımı ve firma hesabına göre Portal taslağı hazırlama üzerinde çalışılmıştı.
- Manuel faturada düzenleyen firma bilgileri, kayıt saklama ve toplu silme bulunuyordu.

Eski prototip JavaScript/Node.js, HTML/CSS ve SQLite kullanıyordu. Bu teknoloji seçimi yeni projeye aktarılmadı. Eski kaynak kodu, veritabanı, fatura kayıtları ve şifreler bu depoya alınmadı.

## Önceki deneyimden hatırlanacak noktalar

Metin ayrıştırmada komşu kayıtlara telefon/plaka taşınması, boş kayıt oluşması ve saat-şehir-tutar birleşiminden yanlış plaka çıkarılması yaşanmıştı. İl/ilçe kısaltmaları ile ödeyen/gönderen ayrımı da önemliydi. Kayıtları işlem öncesinde kontrol edebilmek temel ihtiyaç olarak öne çıkmıştı.

Plaka ve telefonun yoksa boş bırakılabilmesi; varsa doğru kayda bağlanması istenmişti. Eski sürümde eksik TC/VKN için `11111111111` atanması tercih edilmişti. Bu yalnızca geçmiş davranışın kaydıdır; yeni sürüm için alınmış bir karar değildir.

## Canlı sürüm için daha önce konuşulanlar

Kullanıcı hesapları, şirketler arasında veri ayrımı, yönetici/personel yetkileri, PostgreSQL, e-Fatura/e-Arşiv yönlendirmesi, entegratör bağlantısı, belge doğrulama, gönderim kuyruğu, tekrar gönderim koruması, durum takibi, XML/PDF arşivi, iptal/itiraz, yedekleme ve güvenlik konuşulmuştu. Bunlar önceki hedeflerdi; yeni projede hangilerinin ve nasıl uygulanacağı yeniden belirlenecek.

Önceki ana hedef hızlı toplu fatura akışıydı; kapsamlı ön muhasebe, stok ve banka modülleri öncelik olarak belirlenmemişti.

## Belgeler ve kaynak

Önceden “3. Proje başlangıç dosyası - HızlıFatura.docx” ve “4. Gereksinim analizi raporu - HızlıFatura.docx” hazırlanmıştı. Belgeler eski proje klasöründe korunuyor; ayrıca bu çalışmanın yerel çıktılarında referans kopyaları bulunuyor. Kişisel okul bilgileri içeren bu dosyalar GitHub'a yüklenmedi.

Bu not, Codex'teki “Manuel faturaya firma bilgileri ekle” başlıklı konuşmanın son 30 turuna dayanır. Canlı sürüm hedefleri, okul belgeleri, Sheets kararları ve önceki ayrıştırma sorunları incelendi. Konuşmanın bütün eski turlarının incelendiği iddia edilmiyor. Ham konuşmalar ve gerçek müşteri örnekleri depoya aktarılmadı.
