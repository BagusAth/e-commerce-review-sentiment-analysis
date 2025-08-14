# Analisis Sentimen Ulasan Yelp Menggunakan IBM Granite

## 📜 Project Overview

### Latar Belakang
Di era digital, ulasan online menjadi faktor krusial yang memengaruhi reputasi bisnis dan keputusan pembelian konsumen. Platform seperti Yelp menampung jutaan ulasan yang mengandung umpan balik berharga. Namun, menganalisis data dalam volume besar ini secara manual tidaklah efisien.

### Permasalahan
Banyak bisnis, terutama skala kecil dan menengah, kesulitan untuk memahami sentimen pelanggan secara keseluruhan dari ribuan ulasan. Mereka membutuhkan cara otomatis untuk mengekstrak wawasan utama, mengidentifikasi keluhan, dan menemukan pujian untuk membuat keputusan bisnis yang lebih baik.

### Tujuan Proyek
Proyek ini bertujuan untuk membangun sebuah alur kerja analisis data untuk mengklasifikasikan sentimen ulasan dari dataset Yelp secara otomatis. Dengan bantuan model AI Generatif dari IBM, proyek ini akan menghasilkan:
1.  Klasifikasi sentimen (Positive, Negative, Neutral, Mixed).
2.  Ringkasan otomatis dari ulasan.
3.  Insight dan temuan bisnis yang dapat ditindaklanjuti.
4.  Rekomendasi konkret untuk perbaikan bisnis berdasarkan hasil analisis.

## 💾 Link Raw Dataset

Dataset yang digunakan dalam proyek ini adalah **Yelp Reviews Full**. Dataset ini bersifat publik dan dapat diakses melalui Hugging Face.

* **Sumber:** [Yelp Review Full Dataset on Hugging Face](https://huggingface.co/datasets/Yelp/yelp_review_full)

## 💡 Insight & Findings
Berikut adalah temuan-temuan utama yang dihasilkan oleh AI setelah menganalisis ringkasan data sentimen:

---
**(CONTOH OUTPUT DARI AI)**

* **Balanced Customer Feedback:** The sentiment analysis of product reviews on Yelp reveals a balanced customer feedback with 13 negative, 12 positive, and 5 mixed reviews. This indicates that customers have diverse experiences with the product, suggesting both strengths and areas for improvement.
* **Potential for Product Improvement:** With 13 negative reviews, there is an opportunity to address specific concerns raised by dissatisfied customers. Analyzing these reviews can help identify common issues or features that did not meet customer expectations, enabling the business to prioritize enhancements and refine its product offerings accordingly.
* **Strong Satisfaction among Part of the Customer Base:** The high number of positive reviews (12) signifies that a significant portion of customers is satisfied with the product's performance. This finding emphasizes the importance of maintaining and leveraging these positive experiences to build brand loyalty and encourage repeat purchases. Additionally, understanding the nature of these positive reviews can provide valuable insights into successful product features and aspects that contribute to customer satisfaction.

---

## 🚀 Conclusion & Recommendation
Berdasarkan insight yang ditemukan, berikut adalah kesimpulan dan rekomendasi untuk bisnis:
---
**(CONTOH OUTPUT DARI AI)**

### Conclusion
In conclusion, our analysis of customer feedback from Yelp reveals a nuanced picture of product reception, characterized by a mix of positive, negative, and mixed experiences. While a substantial segment of customers expresses satisfaction with the product, there remains a notable proportion expressing dissatisfaction, indicating potential areas for enhancement.

### Recommendations
* **Prioritize Dissatisfied Customers' Concerns :** Given the 13 negative reviews, it is imperative to conduct a thorough investigation into recurring issues or unmet expectations mentioned in these reviews. By addressing these concerns directly, the company can improve product quality and potentially win back dissatisfied customers.
* **Leverage Positive Reviews for Brand Loyalty :** Leverage the success factors highlighted in positive reviews (13 in number) to strengthen marketing strategies and enhance brand positioning. Reinforcing these positive aspects can boost customer confidence and loyalty.
* **Analyze Mixed Reviews for Product Refinement :** Implement a robust feedback loop system to continuously gather, analyze, and act upon customer reviews. This proactive strategy ensures ongoing product refinement, enhances customer satisfaction, and fosters long-term business growth.

By following these recommendations, the company can effectively navigate the current feedback landscape, turning negative perceptions into opportunities for improvement and solidifying its market position through consistent quality delivery.

---

## 🤖 AI Support Explanation

Dalam proyek ini, model AI Generatif **`ibm-granite/granite-3.3-2b-instruct`** dari IBM digunakan sebagai "otak" analisis. Model ini tidak hanya digunakan untuk satu tugas, melainkan untuk beberapa tahapan analisis data secara berurutan:

1.  **Klasifikasi Sentimen:** AI diberi perintah untuk mengklasifikasikan setiap ulasan ke dalam empat kategori (Positive, Negative, Neutral, Mixed) berdasarkan konten teksnya.
2.  **Summarization (Peringkasan):** AI mampu membuat ringkasan singkat dari ulasan yang panjang, mengekstrak poin-poin utamanya.
3.  **Insight Generation:** Setelah data sentimen diagregasi, AI diberi peran sebagai analis data. Ia diberikan ringkasan statistik (misalnya, jumlah ulasan positif dan negatif) dan diminta untuk menghasilkan *insight* atau wawasan bisnis yang mendalam dari angka-angka tersebut.
4.  **Recommendation Generation:** Berdasarkan *insight* yang telah dibuatnya, AI kemudian diberi peran sebagai konsultan bisnis untuk memberikan kesimpulan dan rekomendasi yang konkret dan dapat dijalankan (*actionable*) untuk perbaikan bisnis.
