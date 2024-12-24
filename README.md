# Muhasebe Otomasyonu

Bu proje, kullanıcıların gelir ve gider işlemlerini kaydedebileceği, bakiyeyi takip edebileceği bir muhasebe otomasyonu uygulamasıdır. SQLite veritabanı kullanarak gelir ve gider işlemleri kaydedilir ve güncel bakiye hesaplanır.

## Özellikler

- **Gelir Ekleme**: Kullanıcı, gelir miktarını ve açıklamasını girerek gelir kaydını oluşturabilir.
- **Gider Ekleme**: Kullanıcı, gider miktarını ve açıklamasını girerek gider kaydını oluşturabilir.
- **İşlemleri Listeleme**: Gerçekleştirilen tüm gelir ve gider işlemleri listelenebilir.
- **Bakiye Görüntüleme**: Güncel bakiye kullanıcıya gösterilir.

## Gereksinimler

- Python 3.x
- `sqlite3` modülü (Python ile birlikte gelir)

## Kurulum ve Çalıştırma

1. Python yüklü olduğundan emin olun.
2. Bu projeyi indirip uygun bir klasöre yerleştirin.
3. Aşağıdaki komutla Python dosyasını çalıştırın:

   ```bash
   python muhasebe_otomasyonu.py
   ```

4. Program çalışmaya başladığında, kullanıcıya çeşitli seçenekler sunulacaktır:
    - **1. Gelir Ekle**: Gelir eklemek için bu seçeneği tıklayın.
    - **2. Gider Ekle**: Gider eklemek için bu seçeneği tıklayın.
    - **3. İşlemleri Listele**: Tüm işlemleri listelemek için bu seçeneği tıklayın.
    - **4. Bakiye Görüntüle**: Güncel bakiyenizi görmek için bu seçeneği tıklayın.
    - **5. Çıkış**: Programdan çıkmak için bu seçeneği tıklayın.

## Veritabanı Yapısı

- **transactions**: Gelir ve gider işlemlerini kaydeden tablo.
  - **id**: İşlem ID'si (otomatik artan)
  - **type**: İşlem türü (gelir/gider)
  - **amount**: İşlem miktarı
  - **description**: İşlem açıklaması
  - **date**: İşlem tarihi

- **balance**: Kullanıcı bakiyesini tutan tablo.
  - **id**: Sabit değer, sadece 1 kayıt bulunur.
  - **total_balance**: Toplam bakiye

## Kullanım

1. Gelir veya gider eklemek için ilgili seçeneği seçin ve gerekli bilgileri girin (miktar ve açıklama).
2. İşlemlerinizi görmek için "İşlemleri Listele" seçeneğini seçebilirsiniz.
3. Güncel bakiyenizi görmek için "Bakiye Görüntüle" seçeneğini seçebilirsiniz.
4. Çıkış yapmak için "Çıkış" seçeneğini seçin.

## Katkıda Bulunma

Bu projeye katkıda bulunmak isterseniz, lütfen bir pull request gönderin veya önerilerinizi bizimle paylaşın.

## Lisans

Bu proje, [MIT Lisansı](https://opensource.org/licenses/MIT) altında lisanslanmıştır.

