# 🚀 Scalable Data Pipeline Dashboard
**Developer: Manar Salman | إعداد : منار سلمان**

هذا المشروع هو مختبر تفاعلي لمقارنة أداء معالجة البيانات الضخمة (Big Data) بين المعالجات المركزية التقليدية (CPU) والمعالجات الرسومية المسرّعة (NVIDIA GPU).

---

## 📢 Note on Data Source | ملاحظة حول مصدر البيانات
> [!IMPORTANT]
> **Data Generation:** This project uses a custom Python generator script to create large-scale synthetic datasets. This was done to simulate high-volume real-world scenarios and to benchmark the performance of different processing engines accurately.
> 
> **مصدر البيانات:** يوضح هذا المشروع أن البيانات المستخدمة تم إنشاؤها عبر "مولد بيانات" (Generator) برمجياً، وذلك لمحاكاة بيئات العمل الضخمة واختبار قدرة النظام على التوسع (Scalability).

---

## 🛠️ Tech Stack | التقنيات المستخدمة
* **Pandas:** المعيار الأساسي لمعالجة البيانات (Single-core CPU).
* **Dask:** للحوسبة الموازية وتوزيع المهام (Multi-core CPU).
* **RAPIDS cuDF:** لمعالجة البيانات المسرّعة بواسطة الـ GPU (NVIDIA T4).
* **Gradio:** لبناء الواجهة التفاعلية للمشروع.
* **Plotly:** لإنشاء الرسوم البيانية التفاعلية.

---

## 📊 Key Features | مميزات المشروع
- **Real-time Benchmarking:** مقارنة فورية للأداء عند تغيير حجم البيانات.
- **Interactive UI:** واجهة مستخدم تسمح بتوليد بيانات تصل إلى 10 مليون سطر بضغطة زر.
- **Scalability Analysis:** توضيح كيف يتفوق الـ GPU على الـ CPU مع زيادة حجم البيانات.

[attachment_0](attachment)

---

## 🚀 How to Run | كيف تشغل المشروع
المشروع مصمم ليعمل على **Google Colab** للاستفادة من الـ GPU المجاني:
1. افتح الملف في Google Colab.
2. قم بتغيير نوع وقت التشغيل (Runtime) إلى **T4 GPU**.
3. قم بتشغيل الخلية البرمجية الشاملة.
4. استخدم الرابط العام (Gradio Link) لفتح الواجهة وتجربة الاختبار.

---

## 📈 Performance Result Sample | عينة من نتائج الأداء
| Engine | Time (1M Rows) | Performance |
| :--- | :--- | :--- |
| **Pandas** | ~10.7s | Baseline (Slowest) |
| **Dask** | ~7.9s | 1.3x Faster |
| **cuDF (GPU)** | **~1.1s** | **9.6x Faster!** |

---

## 📜 Conclusion | الخلاصة
أثبت المشروع أن الانتقال من المعالجة التقليدية إلى المعالجة المعتمدة على الـ GPU (عبر مكتبات RAPIDS) يوفر تحسيناً هائلاً في الأداء، مما يجعله الحل الأمثل لخطوط أنابيب البيانات في علوم البيانات والذكاء الاصطناعي.

---
**Prepared with passion by Manar Salman 💻**
