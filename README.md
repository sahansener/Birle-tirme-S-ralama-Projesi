# Merge Sort Projesi

Bu repo, [Patika.dev](https://www.patika.dev/tr) Veri Yapıları ve Algoritmalar eğitimi kapsamında hazırlanan Merge Sort projesidir.

---

## Proje Sorusu

**[16, 21, 11, 8, 12, 22]** dizisinin Merge Sort (Birleştirme Sıralaması) aşamalarını ve Big-O gösterimini yazınız.

---

## 1. Merge Sort Aşamaları

Merge Sort, "Böl ve Yönet" (Divide and Conquer) prensibiyle çalışır. Dizi önce en küçük parçalarına kadar bölünür, sonra sıralanarak birleştirilir.

**Dizinin Bölünme Aşamaları:**
1.  `[16, 21, 11, 8, 12, 22]` (Başlangıç)
2.  `[16, 21, 11]` - `[8, 12, 22]` (Dizi ikiye bölündü)
3.  `[16]` - `[21, 11]` | `[8]` - `[12, 22]` (Alt gruplar bölünmeye devam eder)
4.  `[16]` - `[21]` - `[11]` | `[8]` - `[12]` - `[22]` (Tüm elemanlar tek tek ayrıldı)

**Dizinin Birleşme (Merge) Aşamaları:**
1.  `[16]` - `[11, 21]` | `[8]` - `[12, 22]` (İkili gruplar kendi içinde sıralanarak birleşti)
2.  `[11, 16, 21]` - `[8, 12, 22]` (Üçlü gruplar sıralanarak birleşti)
3.  `[8, 11, 12, 16, 21, 22]` (Tüm dizi küçükten büyüğe sıralı hale geldi)

---

## 2. Big-O Gösterimi

Merge Sort algoritmasında:
* Bölme işlemi her seferinde diziyi ikiye böldüğü için $log(n)$ derinlik oluşur.
* Her derinlikte elemanları karşılaştırıp birleştirmek için $n$ kadar işlem yapılır.

Bu yüzden toplam karmaşıklık:
* **Big-O:** $O(n log n)$

---

## Lisans

Bu proje [MIT](https://choosealicense.com/licenses/mit/) lisansı altındadır.

---

### Hazırlayan:
[Batın]
