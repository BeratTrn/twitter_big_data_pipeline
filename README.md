# ✈️ Twitter Verisi ile Uçtan Uca Büyük Veri Pipeline'ı

Bu proje, **BLG462 - Büyük Veri** dersi dönem projesi kapsamında geliştirilmiş kapsamlı bir ETL (Extract, Transform, Load) ve veri analizi sistemidir. Kaggle üzerinden alınan gerçek Twitter verisi kullanılarak veri temizleme, NoSQL veritabanı modelleme, dağıtık büyük veri işleme ve görselleştirme adımları uçtan uca simüle edilmiştir.

## 🛠️ Kullanılan Teknolojiler
* **Veri İşleme (Transform):** Python, Pandas, Regex
* **Veritabanı (Load & NoSQL):** MongoDB, PyMongo
* **Dağıtık İşleme (Big Data):** PySpark, Spark SQL
* **Görselleştirme:** Matplotlib, Seaborn, WordCloud

## 📂 Proje Mimarisindeki Adımlar
1. **Veri Temini (Extract):** Kaggle üzerinden havayolu şirketlerine ait duygu analizli ~14.000 adet tweet çekilmiştir.
2. **Veri Temizleme (Pandas):** URL, mention, hashtag temizliği yapılmış; eksik veriler doldurularak veri tamlığı ve geçerliliği sağlanmıştır.
3. **MongoDB Modelleme:** Temizlenen veriler NoSQL mimarisine uygun olarak BSON formatında yüklenmiş (Bulk Insert), Aggregation Pipeline ve indeksleme gibi ileri seviye 12 farklı sorgu gerçekleştirilmiştir.
4. **PySpark Dağıtık İşleme:** Veri seti PySpark RDD/DataFrame mimarisine alınarak Transformation ve Action işlemleri uygulanmış, Pandas ile performans kıyaslaması yapılmıştır.
5. **Görselleştirme:** Verideki gizli desenler (Duygu dağılımı, zaman serisi analizi, şikayetlerin kök nedenleri) görselleştirilmiştir.