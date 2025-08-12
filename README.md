# Ogrenci-Basari-Siniflandirmasi
 
Bu projenin amacı, öğrenci verilerini kullanarak öğrencilerin başarı durumlarını (mezuniyet, kayıtlılık veya terk etme) sınıflandırmaktır.

---

## Proje Hakkında
Bu proje, bir öğrenci veri setini kullanarak, öğrencilerin akademik başarı durumlarını tahmin eden bir sınıflandırma modeli geliştirmeye odaklanmaktadır. Veri ön işleme adımları ve veri setinin yapısı hakkında derinlemesine bir analiz içerir.

---

## Kullanılan Teknolojiler
Python: Projenin temel programlama dilidir.

Jupyter Notebook: Kodun yazıldığı ve belgelendiği interaktif ortamdır.

pandas: Veri setini okuma, manipülasyon ve analiz için kullanılan temel kütüphanedir.

scikit-learn: Makine öğrenimi algoritmaları ve veri ön işleme araçları için kullanılır. Özellikle LabelEncoder ve StandardScaler kullanılmıştır.

---

## Veri Seti
Projede kullanılan veri seti data.csv adlı dosyadır. Bu veri seti, öğrencilerin medeni durumları, başvuru bilgileri, kabul notları, demografik bilgileri, ders ünite bilgileri ve sosyoekonomik göstergeler gibi çeşitli özelliklerini içermektedir.

Boyut: Veri seti 4424 satır ve 37 sütundan oluşmaktadır.

Hedef Değişken (Target): Sınıflandırma için kullanılan hedef sütunu, öğrencilerin başarı durumunu gösterir. Bu sütun, "dropout" (terk eden), "enrolled" (kayıtlı) ve "graduate" (mezun) sınıflarını içermektedir.

Veri Dağılımı: Veri setindeki sınıfların dağılımı aşağıdaki gibidir:

Dropout: 1421

Enrolled: 794

Graduate: 2209

## Metodoloji
Veri Yükleme ve Temizleme: data.csv dosyası, pandas kullanılarak okunmuştur. Dosya içeriği noktalı virgül (;) ile ayrıldığı için bu parametre belirtilmiştir. Sütun adlarındaki fazla boşluklar ve kaçış karakterleri temizlenmiştir.

Kayıp Veri Analizi: Veri setinde eksik (null) veri olup olmadığı kontrol edilmiş ve veri setinde eksik veri olmadığı doğrulanmıştır.

Ön İşleme:

Hedef sütun (Target), LabelEncoder kullanılarak sayısal değerlere dönüştürülmüştür.

Sayısal verileri içeren 19 sütun, StandardScaler ile standartlaştırılmıştır.

Son Kontrol: Ön işleme adımları tamamlandıktan sonra, veri setindeki tüm sütunların (float64 veya int64 formatında) makine öğrenimi modeli için uygun hale getirildiği doğrulanmıştır.
