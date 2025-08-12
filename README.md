# Ogrenci-Basari-Siniflandirmasi
 
# Öğrenci Verisi Analizi

Bu proje, öğrenci verilerini içeren bir CSV dosyasını yükleyip ön işleme tabi tutmak ve analiz etmek amacıyla hazırlanmıştır.  
Notebook, verilerin temizlenmesi, dönüştürülmesi ve kaydedilmesi adımlarını içerir.

## İçerik

- **Veri Setini Yükleme:** CSV formatındaki veriler Pandas kütüphanesi kullanılarak yüklenir.
- **Veri Ön İşleme:**
  - Sütun adlarındaki gereksiz boşluklar ve kaçış karakterleri temizlenir.
  - Veriler standart CSV formatında (`students_data.csv`) kaydedilir.
- **İlk İnceleme:** `head()` fonksiyonu ile verinin ilk satırları görüntülenir.

## Gereksinimler

Proje aşağıdaki Python kütüphanelerini kullanmaktadır:

```bash
pip install pandas
