# Telco Müşteri Kaybı Analizi

**Ders:** Veri Madenciliği  
**Araç:** Orange Data Mining Tool

---

## Proje Hakkında

Telekom şirketindeki müşteri kayıplarını (churn) analiz edip tahminleyen bir proje. Veri seti Orange'ın içindeki "Telco Customer Churn" verisi.

---

## Kullanılan Widget'lar

- Data Table (veri kontrol için)
- Impute
- Select Columns
- Distributions
- Scatter Plot
- Data Sampler
- Logistic Regression
- Tree
- Random Forest
- Test and Score
- Confusion Matrix
- Tree Viewer

---

## 1. Kısım - Veri Hazırlama

### Yapılanlar
- Veri yüklendi
- TotalCharges sütunundaki boş değerler Impute ile dolduruldu
- customerID çıkarıldı
- Contract vs Churn grafiği çizildi
- MonthlyCharges vs Tenure grafiği çizildi

### Ekran Görüntüleri

<img width="1916" height="1106" alt="image" src="https://github.com/user-attachments/assets/092d75dc-a39c-4447-81ba-8e62d94d091d" />

<img width="1141" height="742" alt="image" src="https://github.com/user-attachments/assets/e8652237-3329-47b1-ac26-11fe1252c495" />

<img width="1403" height="921" alt="image" src="https://github.com/user-attachments/assets/41d84da4-4988-4458-aad4-8846883bdd9b" />

<img width="997" height="656" alt="image" src="https://github.com/user-attachments/assets/e77c1175-0b69-44c2-ab46-62e0093a4e13" />


### Çıkan Sonuç

Aylık sözleşmesi olan müşteriler en çok ayrılan grup oldu.

---

## 2. Kısım - Modelleme

### Yapılanlar
- Veri %80 eğitim %20 test olarak ayrıldı
- Lojistik Regresyon, Karar Ağacı ve Random Forest modelleri kuruldu
- Accuracy ve AUC değerleri karşılaştırıldı
- En iyi model için karmaşıklık matrisi çıkarıldı
- Karar ağacı görselleştirildi

### Modellerin Başarısı

| Model | Accuracy |
|-------|----------|
| Logistic Regression | 0.747 |
| Decision Tree | 0.807 |
| Random Forest | 0.781] |

### Ekran Görüntüleri

<img width="976" height="658" alt="image" src="https://github.com/user-attachments/assets/85567cc9-cad2-43fa-bcac-bf0e9e7a6832" />


<img width="928" height="451" alt="image" src="https://github.com/user-attachments/assets/64efd48a-fe53-4e1b-a30f-ae0bd821fbc3" />
<img width="932" height="458" alt="image" src="https://github.com/user-attachments/assets/1d7f1237-dfe5-4847-84e9-277decb7a608" />
<img width="928" height="457" alt="image" src="https://github.com/user-attachments/assets/879c2e02-e276-4318-aff2-22a38e219db7" />

### En Riskli Müşteri Profili

Karar ağacına göre aylık sözleşmeli ve fiber internet kullanan müşteriler en riskli grup.


**Grup:** Görkem ön - 446731
