McCulloch-Pitts Modelinin İris Veri Setine Uygulaması
Merhaba, bu not belgesi Manisa Celal Bayar Üniversitesi 2026-2027 öğretim yılı yüksek lisans Yapay Sinir Ağları dersi (Öğr. Gör. Dr. Emrah Kuzu) vize ödevim kapsamında hazırladığım kitap bölümünün kaynak kodlarını ve materyallerini içeriyor.

Projede Ne Yaptım?
Bu çalışmada, yapay zeka tarihinin en temel modellerinden biri olan klasik McCulloch-Pitts (MP) nöronunu alıp UCI İris veri setine uyarladım. Temel amacım, sürekli sayısal verileri binarize (0-1) ederek Setosa türünü diğer çiçek türlerinden ayırt etmekti. Modelin kendi içinde bir öğrenme algoritması olmadığı için, en uygun ağırlıkları bulmak adına 272 farklı kombinasyonu deneyen bir Grid Search (Izgara Arama) mekanizması kurdum.

Veri Seti: UCI İris Veri Seti

Kullanılan Yöntem: Uyarlanmış McCulloch-Pitts Eşik Modeli + Grid Search

Model Başarısı: Doğrulama setinde %96.67, Test setinde ise %93.33 doğruluk.

Dosya Yapısı
YSA_Proje_FurkanAktay.ipynb: Veri ön işleme, modelleme ve grafikleri çizdirme adımlarının tamamını içeren Jupyter Notebook dosyam.

requirements.txt: Kodun sizin bilgisayarınızda da sorunsuz çalışması için gereken Python kütüphanelerinin listesi.

grafikler/: Kod üzerinden ürettiğim ve makalede kullandığım G1-G7 grafiklerinin yüksek çözünürlüklü (300 DPI) halleri.

Nasıl Çalıştırılır?
Kodları kendi bilgisayarınızda test etmek isterseniz, repoyu indirip kütüphaneleri (pip install -r requirements.txt) kurmanız yeterli. Sonrasında Jupyter Notebook'u baştan sona çalıştırabilirsiniz. Rastgelelik içeren adımlarda sonuçların değişmemesi (yeniden üretilebilirlik) için kod içinde random_state=42 kullanılmıştır.