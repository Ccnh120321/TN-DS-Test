# Data Dictionary

## Dataset Overview
Dataset นี้เป็น Mock Data ที่ถูกสร้างขึ้นเพื่อจำลองพฤติกรรมของลูกค้าธุรกิจ Retail SME สำหรับการวิเดราะห์ customer churn

| Column | Data Type | Description |
|--------|--------|--------|
| customer_id | string | รหัสลูกค้า |
| last_purshase_days | integer | integer | จำนวนวันตั้งแต่วันที่ซื้อครั้งล่าสุด |
| total_orders | integer | จำนวนคำสั่งซื้อทั้งหมด |
| total_spent | float | ยอดใช้จ่ายรวม |
| promotion_used | string | ลูกค้าเคยใช้โปรโมชั่นหรือไม่ (yes=เคย, no=ไม่เคย) |
| churn | string | ลูกค้าเลิกซื้อหรือไม่ (yes=เคย, no=ไม่เคย)|

## Business Purpose
### last_purchase_days
ใช้วัดความถี่ในการกลับมาซื้อสินค้า ถ้าลูกค้าไม่ได้มาซื้อสินค้านานอาจมีความเสี่ยงใน Churn สูงขึ้น

### total_orders
ใช้รวบรวมจำนวนคำสั่งซื้อของลูกค้า ถ้ามีจำนวนคำนวนซื้อสูงจะมีโอกาสที่จะกลับมาซื้อซ้ำมากกว่า

### total_spent
ใช้วัดมูลค่าของลูกค้าลูกค้าที่มียอดค่าใช้จ่ายสูงมักกลับมาซื้อซ้ำ

### promotion_used
ใช้วิเคราะห์ว่าโปรโมชั่นมีผลกระทบต่อการรักษาฐานลูกค้า

### churn
เป็น Target variable สำหรับการใช้ในการวิเคราะห์ไมเดล customer churn prediction