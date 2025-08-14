# yokatlas-dataset-2025
yök atlas detaylı üniversite, bölüm, puan vb. datası..

# 📄 CSV Veri Seti İçeriği

Bu veri seti, Türkiye’deki üniversitelerin **2015–2024** yılları arasındaki **kontenjan, yerleşme, puan, sıralama ve tercih istatistiklerini** kapsamaktadır.  
Her satır, **tek bir programın** (ör. "Bilgisayar Mühendisliği – İstanbul Teknik Üniversitesi") yıllara göre istatistiklerini içerir.

---

## 📂 Veri Kategorileri

### 1️⃣ Kimlik ve Tanım Bilgileri
| Sütun Adı  | Açıklama |
|------------|----------|
| `id`       | Kayıt numarası |
| `isim`     | Program adı |
| `universite` | Üniversite adı |
| `sure`     | Program süresi (yıl) |
| `tur`      | Program türü (örgün, ikinci öğretim vb.) |
| `kosullar` | Özel koşullar |
| `siraid`   | Tercih kodu |
| `fakulte`  | Fakülte adı |
| `aciklama` | Program açıklaması |
| `il`       | Şehir |
| `unitur`   | Üniversite türü (devlet, vakıf vb.) |
| `onlisans` | Ön lisans / lisans bilgisi |

---

### 2️⃣ Yıllık Kontenjan ve Yerleşme Bilgileri (2015–2024)
| Örnek Sütun Adı | Açıklama |
|-----------------|----------|
| `kontenjan2024` | 2024 yılı toplam kontenjan |
| `yerlesme2024`  | 2024 yılı toplam yerleşen öğrenci sayısı |
| `birinci2024`   | 2024 yılı birincilerin sayısı |
| `birinciyerlesme2024` | 2024 yılı birincilerden yerleşen öğrenci sayısı |

---

### 3️⃣ Puan ve Sıralama Bilgileri (2015–2024)
| Örnek Sütun Adı | Açıklama |
|-----------------|----------|
| `puan2024`      | 2024 yılı taban puanı |
| `maxpuan2024`   | 2024 yılı yerleşen en yüksek puan |
| `sira2024`      | 2024 yılı taban puana karşılık gelen başarı sırası |
| `birincipuan2024` | 2024 yılı birincilerin puanı |
| `birincimaxpuan2024` | 2024 yılı birincilerden en yüksek puana sahip olanın puanı |

---

### 4️⃣ Tercih İstatistikleri
| Örnek Sütun Adı | Açıklama |
|-----------------|----------|
| `tercihtoplam2023`   | 2023 yılı toplam tercih sayısı |
| `tercihbirinci2023`  | 2023 yılı birinci sıradan yapılan tercih sayısı |
| `tercihilkuc2023`    | 2023 yılı ilk 3 tercihten gelen başvuru sayısı |
| `tercihilkdokuz2023` | 2023 yılı ilk 9 tercihten gelen başvuru sayısı |

---

### 5️⃣ Özel Kontenjanlar (2023–2024)
| Sütun Adı | Açıklama |
|-----------|----------|
| `depremzedekontenjan2024` | Depremzedeler için ayrılan kontenjan |
| `kadinkontenjan2024`      | Kadınlar için özel kontenjan |
| `sehitkontenjan2024`      | Şehit yakınları için kontenjan |
| `depremzedeyerlesen2023`  | Depremzedelerden yerleşen öğrenci sayısı |
| `kadinyerlesen2023`       | Kadınlardan yerleşen öğrenci sayısı |
| `sehityerlesen2023`       | Şehit yakınlarından yerleşen öğrenci sayısı |

---

### 6️⃣ Cinsiyet ve Eğitim Durumu Dağılımı
| Sütun Adı | Açıklama |
|-----------|----------|
| `kiz2023`     | 2023 yılı yerleşen kadın öğrenci sayısı |
| `erkek2023`   | 2023 yılı yerleşen erkek öğrenci sayısı |
| `liseli2023`  | 2023 yılı yerleşen lise son sınıf öğrencisi sayısı |
| `mezun2023`   | 2023 yılı yerleşen lise mezunu sayısı |
| `universiteli2023` | 2023 yılı üniversite öğrencisi sayısı |
| `unimezunu2023`    | 2023 yılı üniversite mezunu sayısı |

---

### 7️⃣ Ek Kontenjan Bilgileri (2018–2023)
| Sütun Adı | Açıklama |
|-----------|----------|
| `ekkontenjan2023`         | Ek yerleştirme kontenjanı |
| `eksehitkontenjan2023`    | Ek şehit kontenjanı |
| `ekkadinkontenjan2023`    | Ek kadın kontenjanı |
| `ekdepremzedekontenjan2023` | Ek depremzede kontenjanı |

---

## 📌 Yıllık Kapsam
Veri seti **2015** yılından başlar ve **2024** yılına kadar olan tüm yıllara ait bilgileri içerir.  
Bu sayede:
- 📈 **Puan ve sıralama trendleri**
- 🎯 **Kontenjan değişimleri**
- 👥 **Öğrenci profili analizi**
- 📊 **Cinsiyet ve mezuniyet dağılımı**  
gibi analizler yapılabilir.

