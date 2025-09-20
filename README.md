# Global AI Hub Veri Analizi Projesi

Bu proje, [Powerlifting Database](https://www.kaggle.com/datasets/dansbecker/powerlifting-database) veri seti üzerinde veri analizi ve veri temizleme tekniklerini öğrenmek ve uygulamak amacıyla yapılmıştır.  

Projenin Kaggle notebookuna buradan ulaşabilirsiniz:  
[Global AI Hub Veri Analizi Projem](https://www.kaggle.com/code/sudenazekerci/global-ai-hub-veri-analizi-projem#en-az-bir-tane-eksik-olanlar)

---

## 📊 Proje Adımları

1. **Veri Yükleme ve İnceleme**
   - Veri setini Kaggle üzerinden yükledim.
   - Veri setindeki satır, sütun sayısı, veri tipleri ve ilk 5 satır gibi temel özellikleri inceledim.

2. **Eksik Verilerin Analizi**
   - Eksik değerleri tespit ettim.
   - Her bir değişken için, eksik değerlerin toplam içindeki yüzdesini hesapladım.
   - Eksik olmayan verilerin sayısını ve oranlarını ayrı ayrı inceledim.

3. **Eksik Verilerin Görselleştirilmesi**
   - `missingno` kütüphanesini kullanarak eksik verileri görselleştirdim.
   - `msno.matrix()` ile değişkenler arasındaki eksik değer ilişkilerini gözlemledim.  
     1’e yakın olanların ilişkili olma ihtimalinin yüksek, 0’a yakın olanların ise etkisinin düşük olduğunu değerlendirdim.

4. **Eksik Verilerin Doldurulması ve Silinmesi**
   - Eksik verileri doldurmak için veri setimin kopyasını oluşturdum.
   - Sayısal değişkenlerde **ortalama (mean)** ile doldurma işlemi yaptım.
   - `WeightClassKg` gibi kategorik değişkenleri **mode (mod değeri)** ile doldurdum.
   - İlgisiz eksik verileri sildim.

5. **Kategorik Verilerin İncelenmesi**
   - `division` gibi kategorik değişkenleri analiz ettim.
   - Kategorik değişkenlerin sayısını ve dağılımlarını gözlemledim.
   - Ordinal değerler oluşturarak verileri dönüştürdüm.

6. **Aykırı Değer Analizi**
   - Aykırı değerleri tespit etmek için **IQR (Interquartile Range)** yöntemini kullandım.
   - Alt ve üst sınırları belirledim.
   - **Boxplot** grafikleri ile aykırı değerleri görselleştirdim.
   - Aykırı değerleri veri setinden çıkardım.

7. **Veri Setinin Son Hali**
   - Tüm işlemlerden sonra veri setinin son halini gözlemledim ve tekrar çağırdım.

---

## 🛠 Kullanılan Kütüphaneler

- **pandas**
- **numpy**
- **matplotlib**
- **seaborn**
- **missingno**

---

## 🤖 Not

Projenin geliştirilmesi sırasında **yapay zekadan destek alınmıştır**. Zaten projem öğrenme amaçlı  ve kendi eğitimim için yapılmıştır.

---
