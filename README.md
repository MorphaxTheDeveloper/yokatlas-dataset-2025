# Yök atlas dataset

Bu proje, Türkiye’deki üniversiteler ve programlarına ait **iki farklı veri setini** içerir:

1. **Program Bazlı İstatistikler (2015–2024)**
2. **Üniversite Genel Bilgileri ve Akademik Personel/Öğrenci Sayıları**

---

## 1. Program Bazlı İstatistikler (2015–2024)

Bu CSV, her satırda tek bir programın (ör. *Bilgisayar Mühendisliği – İstanbul Teknik Üniversitesi*) yıllara göre kontenjan, yerleşme, puan, sıralama ve tercih istatistiklerini içerir.

###  Örnek Bilgi Türleri
- Program kimlik ve tanım bilgileri
- Yıllık kontenjan ve yerleşme sayıları
- Taban puan ve sıralama verileri
- Tercih istatistikleri
- Özel kontenjan bilgileri (depremzede, kadın, şehit vb.)
- Cinsiyet ve mezuniyet durumu dağılımı
- Ek kontenjan istatistikleri

> **Ana sütun grupları**  
> `id`, `isim`, `universite`, `sure`, `tur`, `kosullar`, `siraid`, `fakulte`, `aciklama`, `il`, `unitur`, `onlisans`,  
> `kontenjanYYYY`, `yerlesmeYYYY`, `puanYYYY`, `siraYYYY`, `maxpuanYYYY`,  
> `tercihtoplamYYYY`, `kizYYYY`, `erkekYYYY`, `liseliYYYY`, `mezunYYYY`,  
> `depremzedekontenjanYYYY`, `kadinkontenjanYYYY`, `sehitkontenjanYYYY`,  
> `ekkontenjanYYYY`, `eksehitkontenjanYYYY`, `ekkadinkontenjanYYYY`, `ekdepremzedekontenjanYYYY`  
> *(YYYY → yıl: 2015–2024)*

---

## 2. Üniversite Genel Bilgileri

Bu CSV, üniversitelerin temel bilgileri, iletişim bilgileri, akademik personel sayıları ve öğrenci istatistiklerini içerir.

### Örnek Bilgi Türleri
- Üniversite kimlik bilgileri
- İletişim ve konum bilgileri
- Akademik personel dağılımı
- Eğitim seviyelerine göre öğrenci sayıları

> **Ana sütunlar**  
> `isim`, `slug`, `kurulus`, `tur`, `il`, `bolge`, `website`, `eposta`, `telefon`, `fax`, `adres`, `rektor`,  
> `profesor`, `docent`, `doktor`, `ogretim`, `arastirma`,  
> `onlisanserkek`, `onlisanskadin`, `onlisanstoplam`,  
> `lisanserkek`, `lisanskadin`, `lisanstoplam`,  
> `yukseklisanserkek`, `yukseklisanskadin`, `yukseklisanstoplam`,  
> `doktoraerkek`, `doktorakadin`, `doktoratoplam`,  
> `toplamerkek`, `toplamkadin`, `toplam`
# Üniversite genel bilgileri
df_uni = pd.read_csv("universite_bilgileri.csv")

# 2024 yılı en yüksek taban puana sahip ilk 5 program
print(df_program.sort_values("puan2024", ascending=False).head(5))

# En çok lisans öğrencisine sahip 10 üniversite
print(df_uni.sort_values("lisanstoplam", ascending=False).head(10))
