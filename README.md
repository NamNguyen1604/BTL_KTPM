# BÀI TẬP LỚN MÔN: KIỂM THỬ PHẦN MỀM

## I. THÔNG TIN SINH VIÊN TRÌNH BÀY
* **Họ và tên:** Nguyễn Phương Nam
* **Mã số sinh viên (MSV):** K225480106092
* **Ngành học:** Kỹ thuật Máy tính
* **Chuyên ngành:** Công nghệ phần mềm 

## II. GIỚI THIỆU ĐỀ BÀI (ĐỀ TÀI 73)
* **Tên đề tài:** Kiểm thử khả năng truy cập và thiết kế bao trùm trong đảm bảo chất lượng phần mềm (Accessibility Testing & Inclusive Design in Software Quality Assurance).
* **Mục tiêu nghiên cứu & Thực hành:**
    * Nghiên cứu lý thuyết nền tảng về Kiểm thử khả năng truy cập (Accessibility Testing) và Triết lý Thiết kế bao trùm (Inclusive Design) bám sát các giáo trình chuyên ngành **S1 (Chương 5)** và **S4 (Chương 1)**.
    * Thấu hiểu và áp dụng bộ tiêu chuẩn quốc tế **WCAG 2.1 / 2.2** với 4 nguyên tắc cốt lõi **P.O.U.R** (Perceivable - Có thể nhận thức, Operable - Có thể vận hành, Understandable - Có thể hiểu, Robust - Mạnh mẽ).
    * Thiết lập và triển khai bảng Checklist thực nghiệm đo lường chất lượng giao diện phần mềm, tối ưu hóa chi phí sửa lỗi sớm theo nguyên lý **Shift-Left Testing**.
* **Phạm vi thực hành dự án:** * Xây dựng trang web giả lập môi trường giao diện hệ thống thông tin TNUT trên môi trường lập trình **Visual Studio Code (VS Code)**.
    * Triển khai đo lường tự động qua công cụ **Google Lighthouse (Accessibility)** kết hợp kịch bản kiểm thử hộp đen thủ công bằng bàn phím (Keyboard Navigation) để định vị lỗi, thực hiện vá lỗi (Bug fixing) trực tiếp trong mã nguồn HTML/CSS nhằm đưa chất lượng tiếp cận đạt điểm số tuyệt đối 
Kiểm thử tự động:
-Trên trình duyệt , nhấn F12 -> chọn tab Lighthouse -> tích chọn duy nhất ô Accessibility -> bấm Analyze page load. 
<img width="570" height="512" alt="image" src="https://github.com/user-attachments/assets/6e3d3d95-c447-4da3-beb4-f5b5322d95ff" />
<img width="1920" height="1010" alt="image" src="https://github.com/user-attachments/assets/e9c675ed-1117-4c14-99ce-3d1d30780f2c" />
<img width="1920" height="1011" alt="image" src="https://github.com/user-attachments/assets/baf5b09e-95c6-4b4d-a2d5-7668f7f3b87b" />
- Sau khi ấn Ânlyze page load thì sẽ thấy vòng tròn điểm số hiện màu cam hiện 71 điểm do dính lỗi chữ mờ và thiếu alt
<img width="959" height="495" alt="image" src="https://github.com/user-attachments/assets/a3d8e2bf-fa9d-41db-9fcf-8b00e4510d0a" />

Kiểm thử thủ công:
<img width="959" height="506" alt="image" src="https://github.com/user-attachments/assets/5b18dcec-b78d-498b-8bc1-ed680d47d16b" />
- Khi click chuột lên thanh địa chỉ trình duyệt, sau đó nhấn phím Tab liên tục. ẽ thấy con trỏ nhảy qua "Trang chủ", "Tin tức tuyển sinh" nhưng không hề có viền khung nào sáng lên. -> Ghi nhận lỗi mất dấu tiêu điểm.

Giai đoạn 2: Sửa lỗi trực tiếp trên VS Code để đạt chuẩn
Lỗi 1: Độ tương phản chữ mờ
<img width="1920" height="1003" alt="image" src="https://github.com/user-attachments/assets/91a50a3c-f7cf-41b3-a4d3-01e972962a40" />
Lỗi 2: Mất tiêu điểm bàn phím
<img width="1920" height="1006" alt="image" src="https://github.com/user-attachments/assets/774b41eb-271f-4c24-aaca-956352392c08" />
Lỗi 3: Thiếu mô tả hình ảnh
<img width="661" height="105" alt="image" src="https://github.com/user-attachments/assets/f88e0d4d-1d6d-4cae-aa34-75759175e53e" />
- Sau khi sửa thì kết quả đã mang lại tốt hơn : 
<img width="958" height="475" alt="image" src="https://github.com/user-attachments/assets/33675703-31c2-479e-b00b-8036690c6515" />

<img width="959" height="475" alt="image" src="https://github.com/user-attachments/assets/9e05b7cf-2f18-4aff-938f-a051704c949f" />
Kết quả sau khi tối ưu: Điểm số Accessibility trên Lighthouse đạt mức tuyệt đối 100 / 100 điểm.

Đánh giá rủi ro tồn dư (Residual Risk): Rủi ro giảm từ mức Cao (Critical) xuống mức Thấp/Triệt tiêu (Negligible). Trang web hoàn toàn đủ điều kiện để đưa vào vận hành thực tế đáp ứng triết lý Thiết kế bao trùm (Inclusive Design).
