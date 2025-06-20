# Data-Warehouse-design
# 📊 Data Mart – Phòng Tài Chính – Kế Toán

## 🎯 Mục tiêu dự án
Xây dựng một Data Mart phục vụ phân tích tài chính – kế toán cho công ty thương mại điện tử, hỗ trợ phòng kế toán trả lời các câu hỏi nghiệp vụ như:

- Doanh thu theo thời gian, khách hàng, sản phẩm
- Giá trị hoàn tiền theo tháng/quý
- Theo dõi công nợ khách hàng
- Báo cáo tổng hợp kế toán sổ cái

## 📈 Câu hỏi phân tích chính

1. Tổng doanh thu theo ngày, tháng, năm là bao nhiêu?
2. Khách hàng nào mang lại doanh thu cao nhất?
3. Tỷ lệ hoàn tiền là bao nhiêu? Nhóm sản phẩm nào bị hoàn nhiều nhất?
4. Tổng công nợ phải thu là bao nhiêu? Theo từng khách hàng?
5. Tổng số tiền ghi nhận vào từng tài khoản kế toán (GL) là bao nhiêu?

## 🧱 Định hướng thiết kế dữ liệu

### Fact Tables
- `fact_revenue`
- `fact_refund`
- `fact_receivable`
- `fact_gl_summary`

### Dimension Tables
- `dim_customer`
- `dim_date`
- `dim_product`
- `dim_account`

## 📦 Nguồn dữ liệu giả định
- orders.csv, refunds.csv, payments.csv, journal_entries.csv,...
