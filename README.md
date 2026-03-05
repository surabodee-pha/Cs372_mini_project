# CS372 Mini Project 1 — WFH Burnout Risk Classification

> **การจำแนกประเภทความเสี่ยงภาวะหมดไฟจากการทำงานที่บ้าน**  
> ด้วยเทคนิค Machine Learning: kNN · XGBoost · Neural Network

---

## 👥 รายชื่อสมาชิกกลุ่ม

| ลำดับ | ชื่อ-นามสกุล | เลขทะเบียนนักศึกษา |
|:---:|:---|:---:|
| 1 | นายรพินทร์ นะราช | 6609650624 |
| 2 | นายสุทธิพจน์ ประทุมทอง | 6609650699 |
| 3 | นายสุรบดี ผาสุข | 6609650707 |

---

## 📝 เกี่ยวกับโปรเจกต์

โปรเจกต์นี้พัฒนาแบบจำลอง **Classification** เพื่อทำนายระดับความเสี่ยงภาวะ Burnout ของพนักงาน Work From Home โดยใช้ข้อมูลพฤติกรรมการทำงานประจำวัน เช่น ชั่วโมงการทำงาน การนอนหลับ และคะแนนความเหนื่อยล้า

**Target:** `burnout_risk` → `Low` / `Medium` / `High`

| รายการ | รายละเอียด |
|:---|:---|
| Dataset | `wfh_burnout_dataset 19.19.18.csv` |
| จำนวนข้อมูล | 2,000 records · 14 columns |
| Feature Selection | Tree-based + Permutation Importance (2/3 Rule) |
| Validation | 5-Fold Stratified Cross Validation |
| Train/Test Split | 80% / 20% |

---

## 📊 ผลลัพธ์สรุป (Results)

| โมเดล | CV Accuracy | Test Accuracy |
|:---|:---:|:---:|
| k-Nearest Neighbors (kNN) | 0.9675 ± 0.0116 | 0.9700 |
| **XGBoost** ⭐ | **0.9994 ± 0.0013** | **1.0000** |
| Neural Network (MLP) | 0.9769 ± 0.0094 | 0.9725 |

*Thammasat University · Bachelor of Science in Computer Science · CS372 Machine Learning · 2/2567*
