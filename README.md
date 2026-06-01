# Telco Churn Analizi - 1. Kısım

## Veri Yükleme
Telco Customer Churn verisi Orange'daki Datasets widget ile yüklendi.

## Veri Denetimi
Data Table ile bakınca TotalCharges sütununun text olarak geldiğini gördüm. Nedeni bu sütunda boş değerler olması.

## Temizlik
- **Impute** ile boş değerler dolduruldu. Sayısal sütunlar için ortalama kullanıldı.
- **Select Columns** ile customerID devre dışı bırakıldı.

## Grafikler ve Yorum
Araştırmalar gösteriyor ki Month-to-month sözleşmesi olan müşteriler en yüksek churn oranına sahiptir . Bunun nedeni, bu müşterilerin herhangi bir cayma cezası olmadan istedikleri zaman servisi bırakabilmeleri, 1 veya 2 yıllık sözleşmesi olan müşterilerin ise daha uzun taahhütleri nedeniyle daha düşük churn oranı göstermesidir 

### Contract vs Churn
Distributions grafiğinde en çok ayrılanların month-to-month sözleşmesi olanlar olduğu görüldü. Yıllık sözleşmelerde churn oranı daha düşük.

### MonthlyCharges vs Tenure
Scatter Plot'ta tenure düşük ve monthlyCharges yüksek olan müşterilerde churn daha fazla.

## Temizlenmiş Veri
TotalCharges artık sayısal görünüyor, boş değer kalmadı.

## Workflow
Datasets → Impute → Select Columns → Distributions / Scatter Plot / Data Table

![alt text](image.png)
![alt text](image-1.png)

---

**Grup:** Görkem Ön - 446731
