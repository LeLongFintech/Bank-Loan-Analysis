# Bank Loan Analysis

Dự án phân tích nhỏ sử dụng Python & pandas để theo dõi KPI, xu hướng theo thời gian và các phân tích phân tầng (theo bang, thâm niên làm việc, kỳ hạn vay, hình thức sở hữu nhà).

---

## 🎯 Bài toán (Problem Statement)

Mục tiêu là trả lời các câu hỏi kinh doanh và trực quan hóa sau:

- **KPI cốt lõi**  
  - Tổng số **Loan Applications** (bao gồm **MTD**)  
  - **Total Funded Amount** (bao gồm **MTD**)  
  - **Total Amount Received** (bao gồm **MTD**)  
  - **Average Interest Rate**, **Average DTI**

- **Nhóm “Good vs Bad” loans**  
  - Định nghĩa (tham khảo trong notebook):  
    - **Good**: `loan_status ∈ {Current, Fully Paid}`  
    - **Bad**: các trạng thái còn lại  
  - Với mỗi nhóm: Tỷ trọng đơn, số đơn, tổng giải ngân, tổng thu về

- **Biểu đồ yêu cầu**  
  - Xu hướng theo **Issue Date** (theo tháng)  
  - **Regional Analysis** theo `address_state`  
  - **Loan Term** (donut) — 36 vs 60 tháng  
  - **Employment Length** (bar) — các nhóm: `< 1`, `1–3`, `3–5`, `5–7`, `7–9`, `10+` năm  
  - **Home Ownership** (treemap/heatmap) — phân bổ giải ngân theo `home_ownership`

---

## 🗂 Cấu trúc kho mã
├─ financial_loan.ipynb # Notebook chính (toàn bộ xử lý & biểu đồ)
├─ financial_loan.xlsx # Dữ liệu đầu vào
├─ Problem Statement.pdf # Yêu cầu/bối cảnh bài toán
└─ README.md
