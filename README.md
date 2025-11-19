# 🛒 Portfolio Dự án Kiểm thử Thanh toán E-commerce – Shopee

## 🔰 Giới thiệu
Dự án này là phân tích chuyên sâu và thiết kế Test Case cho tính năng **Thanh toán (Checkout)** trên ứng dụng **Shopee**, nhằm đảm bảo tính chính xác, an toàn và hiệu quả của luồng giao dịch.  
Dự án được thực hiện để chứng minh khả năng phân tích các yêu cầu nghiệp vụ phức tạp, đặc biệt là các **ràng buộc tài chính**, **bảo mật**, và **đa phương thức thanh toán**.

---

## I. 🎯 Các Tính Năng Kiểm Thử Cốt Lõi

Dự án tập trung vào **6 lĩnh vực kiểm thử chính**, bám sát các yêu cầu nghiệp vụ:

| **Lĩnh vực** | **Mục tiêu kiểm thử** | **Kỹ năng chính** |
|--------------|------------------------|-------------------|
| **A. Dữ liệu Hóa đơn** | Tính đúng Tổng tiền, VAT (10%), phí vận chuyển, Tổng thanh toán. | Black Box (EP/BVA), Functional |
| **B. Mã giảm giá (Voucher)** | Kiểm tra logic voucher 5% (Shop), 12% (Sàn), và ràng buộc giá trị tối thiểu 100.000đ. | Decision Table, Functional |
| **C. Đa phương thức thanh toán** | Xác minh hỗ trợ 4 phương thức: Thẻ, Ví điện tử, Chuyển khoản, COD. | Functional, Compatibility |
| **D. Quy trình Thanh toán** | Kiểm tra đầy đủ workflow từ chọn phương thức → xử lý giao dịch → gửi email xác nhận. | Workflow Testing |
| **E. Ràng buộc Nghiệp vụ** | Giới hạn 50 triệu/ giao dịch, Timeout 15 phút/phiên, giới hạn khu vực COD. | Constraint, Boundary |
| **F. Bảo mật & Rủi ro** | Kiểm tra 3D Secure (Thẻ quốc tế), OTP Ví điện tử, Negative security cases. | Security Testing |

---

## II. ⚠️ Ràng Buộc Nghiệp Vụ Cần Chú Trọng (Constraint Testing)

Dự án tập trung vào việc phân tích và kiểm thử các ràng buộc quan trọng:

- **Giới hạn tiền:** tối đa **50.000.000 VNĐ** cho mỗi giao dịch.  
- **Thời gian Timeout:** **15 phút** cho mỗi phiên thanh toán.  
- **COD:** chỉ áp dụng trong **nội thành Hà Nội và TP. HCM**.  
- **Thẻ quốc tế:** bắt buộc xác thực **3D Secure**.  

---

## III. 📄 Tài Liệu Kiểm Thử (Artifacts)

Bộ tài liệu kiểm thử đã được xây dựng đầy đủ, sẵn sàng dùng cho phỏng vấn:

| **Tài liệu** | **Mô tả** |
|--------------|-----------|
| **Test Plan** | Xác định phạm vi, chiến lược và hướng tiếp cận 6 lĩnh vực kiểm thử. |
| **Test Cases** | Tập trung Black Box Testing cho Voucher, Constraint (50M, 15 phút, COD), 3D Secure. |


---

## 👤 Tác Giả
- **Lê Đức Kiên** 

---
