# Retail Customer Churn Analysis

## Project Overview
ธุรกิจ Retail SME มีกสูญเสียรายได้จากลูกค้าที่เลิกซื้อสินค้าโดยไม่ทราบล่วงหน้า ทำให้ไม่สามารถดำเนินมาตรการดำเนินการรักษาลูกค้าได้ทันที

โดย Project นี้นำเสนอแนวทางการใช้ Data Science และ AI เพื่อวิเคระห์พฤติกรรมและระบุปัจจัยที่เกี่ยวข้องกับ Customer Churn โดยมีเป้าหมายเพื่อช่วยให้ธุรกิจรักษาฐานลูกค้าได้

---

## Business Preblem
### Preblem Statement
ร้านค้าปลีก SME สูญเสียรายได้จากลูกค้าที่เลิกซื้อสินค้าโดยไม่ทราบล่วงหน้า

### Target Users
- Marketing Team
- Business Owner

### Business Goal
ลดอัตราการสูญเสียลูกค้า

### KPIs
- Customer Retention Rate
- Customer Churn Rate

---

## Proposed DS / AI Solution

วิเคราะห์ข้อมูลลูกค้าเพื่อค้นหาปัจจัยที่เกี่ยวข้องกับการเสียลูกค้า เช่น 
- ระยะเวลาตั้งแต่การซื้อครั้งล่าสุด
- จำนวนคำสั่งซื้อสินค้าทั้งหมด
- ยอดใช้จ่ายรวม
- การใช้โปรโมชั่น

ผลลัพธ์ที่ได้สามารถนำไปใช้ออกแบบกลยุทธ์ทางการตลาดได้

### Input
- Customer Transaction Date
- Purchase History
- Promation Usage Data

### Output
- Churn Indicators
- Business Insights

## Project Structure
```test
TN-DS-Test
│
├── retail_churn_prediction.ipynb
├── customer_data_mock.csv
├── docs
│   ├── data_dictionary.md
│   └── pseudo_code.md
└── README.md
```

## Dataset
Dataset ที่ใช้เป็น Mock Data ที่สร้างขึ้นเพื่อจำลองพฤติกรรมของลูกค้าในธุรกิจ Retail SME

### Main Features

| Feature | Description |
|---------|---------|
| customer_id | รหัสลูกค้า |
| last_purchase_days | จำนวนวันตั้งแต่ซื้อครั้งล่าสุด |
| total_orders | จำนวนคำสั่งซื้อทั้งหมด |
| total_spent | ยอดใช้จ่ายรวม |
| promotion_used | เคยใช้โปรโมชั่นหรือไม่ |
| churn | ลูกค้าเลิกซื้อหรือไม่ |

## Analysis Process
1. Data Quality Check
2. Data Cleaning
3. Explortory Data Analysis
4. Customer Behavior Analysis
5. Business Insight Generation

## Key Findings
จากการวิเคราห์ข้อมูลตัวอย่างพบว่า:
- ลูกค้าที่ไม่ได้ซื้อสินค้านานมีแนวโน้ม Churn สูงกว่า
- ลูกค้าที่มีจำนวนคำสั่งซื้อสูงมีแนวโน้มที่จะกลับมาซื้ออีก
- ลูกค้าที่มีค่าใช้จ่ายสูงมีโอกาสที่จะกลับมาซื้อซ้ำ
- การทำโปรโมชั่นช่วยลดความเสี่ยงที่จะสูญเสียลูกค้าได้

---

## AI Tools Used
- ChatGPT: ช่วยในการจัดการโครงสร้าง Project ตรวจความสมเหตุสมผลของ dataset ช่วยเรียบเรียงคำและตรวจสอบความถูกต้อง
- Gemini: ช่วยในการหาข้อมูลเกี่ยวกับ Retail SME
