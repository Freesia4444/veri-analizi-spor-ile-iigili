kaggledaki notebookum-->https://www.kaggle.com/code/sudenazekerci/global-ai-hub-veri-analizi-projem#en-az-bir-tane-eksik-olanlar.
bu veri setimde boy kilo cinsiyet gibi veriler içeren bir veri seti kullandım. veri seti--> https://www.kaggle.com/datasets/dansbecker/powerlifting-database

bu veri setini yaparken ilk başta eksik veriler oluşturdum , verimin satır ve sutununu analiz ettim ilk 5 verisini, veri türlerimi kolon sayısı gibi şeyleri gözlemledim .
eksik verilerime baktım ve Her bir değişken için, o değişkendeki eksik değer sayısının toplam kayıt sayısının % kaçı olduğunu buldum.
ardından eksik olmayanları ayırt ettim ve sayılarına baktım.
ardından missinganko kutuphanesini ekledim ve görselleştirdim.
msno.matrix(), değişkenlerde bulunan eksik değerlerin ilişkili olup olmadığını görsel yolla tespit ettim.
buradan 1 e yakın olanların ilişki ihtimallerinin yüksek 0 a yakın olanlarınında etkisi olmadığı bilgisini kullanarak gözlemledim,eksik verilerimi sildim.
doldurma işlemini gerçekleştirmek için veri setimin kopyasını oluşturdum.
Bir sayısal değişkenin dağılımını görmek için histogram kullandım.
ilk başta kategorik verilerim yokmuş gibi gözüktü ardından ben de sayısal verilerimi doldurdum ve yine ardından önceki ile doldurma işlemini yaptım.
mode değeri ile doldurdum WeightClassKg yi.
kategorik verilere baktım ve division adlıyı inceledim, kategorik değişkenlerin sayısına baktım.
ordinal değer oluşturdum.
Ardından veri çerçevesini yükledikten sonra işlemi gerçekleştirdim ve ilk 5 satırı kontrol ettim.
Bir değişkendeki IQR'a göre aykırı gözlemleri boxplot kullanarak görselleştirdim ve Quantile değerlerin belirlenmesi.IQR değerin belirlenmesi.Alt ve üst sınırların belirlenmesi gibi işlemleri de yaptım, aykırı 
gözlemleri sildim.
Ve en son  veri sonuçlarımı tekrar cağırdım.
