# Analisis Sentimen Ulasan E-commerece(Yelp) Menggunakan IBM Granite

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

* **Balanced Customer Feedback:** The data indicates a balanced distribution of reviews with 15 negative, 13 positive, 1 neutral, and 1 mixed. This suggests that customers have diverse experiences with product Y, ranging from satisfactory to dissatisfaction. A balanced feedback is generally positive as it signifies that the product meets or exceeds customer expectations in most cases, while also acknowledging areas for improvement.
* **Potential for Product Improvement:** With 15 negative reviews outweighing the positive ones, there is an opportunity for product enhancement. These negative reviews may highlight specific pain points or dissatisfactions that need addressing. Analyzing these reviews can provide valuable insights into recurring issues, enabling targeted improvements to enhance overall customer satisfaction and loyalty.
* **Engagement and Satisfaction Levels:** The presence of both positive (13) and negative (15) reviews implies varying levels of engagement and satisfaction among users. To capitalize on this, businesses should focus on understanding the reasons behind positive reviews to reinforce successful aspects and address concerns raised in negative reviews to mitigate dissatisfaction. This approach will help in crafting tai

---

## 🚀 Conclusion & Recommendation
Berdasarkan insight yang ditemukan, berikut adalah kesimpulan dan rekomendasi untuk bisnis:
---
**(CONTOH OUTPUT DARI AI)**

### Conclusion
In conclusion, the analysis of customer feedback reveals a complex picture of product Y's performance, marked by a mix of positive, negative, neutral, and mixed reviews. While the majority of customers seem satisfied (13 positive and 1 neutral/mixed), the prevalence of negative reviews (15) underscores significant room for improvement. These negative reviews serve as critical feedback channels, highlighting potential product shortcomings and areas requiring attention.By following these recommendations, the company can effectively navigate the current feedback landscape, turning negative perceptions into opportunities for improvement and solidifying its market position through consistent quality delivery.

### Recommendations
* Conduct a thorough analysis of negative reviews to identify common themes and recurring issues. Prioritize these findings to develop targeted solutions addressing the core concerns of dissatisfied customers.
* Leverage the success factors highlighted in positive reviews (13 in number) to strengthen marketing strategies and enhance brand positioning. Reinforcing these positive aspects can boost customer confidence and loyalty.
* Implement a robust feedback loop system to continuously gather, analyze, and act upon customer reviews. This proactive strategy ensures ongoing product refinement, enhances customer satisfaction, and fosters long-term business growth.

By following these recommendations, the company can effectively navigate the current feedback landscape, turning negative perceptions into opportunities for improvement and solidifying its market position through consistent quality delivery.

---

## 🤖 AI Support Explanation

Dalam proyek ini, model AI Generatif **`ibm-granite/granite-3.3-2b-instruct`** dari IBM digunakan sebagai "otak" analisis. Model ini tidak hanya digunakan untuk satu tugas, melainkan untuk beberapa tahapan analisis data secara berurutan:

1.  **Klasifikasi Sentimen:** AI diberi perintah untuk mengklasifikasikan setiap ulasan ke dalam empat kategori (Positive, Negative, Neutral, Mixed) berdasarkan konten teksnya.
2.  **Summarization (Peringkasan):** AI mampu membuat ringkasan singkat dari ulasan yang panjang, mengekstrak poin-poin utamanya.
3.  **Insight Generation:** Setelah data sentimen diagregasi, AI diberi peran sebagai analis data. Ia diberikan ringkasan statistik (misalnya, jumlah ulasan positif dan negatif) dan diminta untuk menghasilkan *insight* atau wawasan bisnis yang mendalam dari angka-angka tersebut.
4.  **Recommendation Generation:** Berdasarkan *insight* yang telah dibuatnya, AI kemudian diberi peran sebagai konsultan bisnis untuk memberikan kesimpulan dan rekomendasi yang konkret dan dapat dijalankan (*actionable*) untuk perbaikan bisnis.
