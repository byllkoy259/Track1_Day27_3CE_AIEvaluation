# CS12 · AI Evaluation

**Tên nhóm:** 3CE

## Thành viên

| STT | Họ tên | MSSV |
|---|---|---|
| 1 | Vũ Quốc Bảo | 2A202602829 |
| 2 | Hà Thị Mỹ Linh | 2A202602619 |
| 3 | Đỗ Thanh Lâm | 2A202602577 |
| 4 | Đào Trọng Khang | 2A202602974 |

## Phân công nhiệm vụ (đề xuất)

| Thành viên | Nhiệm vụ |
|---|---|
| Vũ Quốc Bảo | Điều phối nhóm, xác định mục tiêu và tiêu chí đánh giá AI; tổng hợp kế hoạch. |
| Hà Thị Mỹ Linh | Thu thập, rà soát tài liệu và chuẩn bị dữ liệu hoặc bộ câu hỏi đánh giá. |
| Đỗ Thanh Lâm | Thực hiện đánh giá AI theo tiêu chí; ghi lại kết quả và các trường hợp lỗi. |
| Đào Trọng Khang | Phân tích kết quả, viết báo cáo và chuẩn bị phần trình bày. |

## Ghi chú rà soát bộ đề (Hà Thị Mỹ Linh · X2, X3)

- **X2 · Chiều và phễu:** giữ 3 chiều Ý định (4) × Độ đủ thông tin (3) × Tình trạng đơn (3) = 36 tổ hợp, loại 12 tổ hợp phi lý còn 24, chọn 16 tình huống × 3 cách diễn đạt = 48 đầu vào. Cả 3 chiều đều qua phép thử (đổi giá trị thì hành vi đúng đổi).
- **X3 · 8 tình huống:** 3 đại diện, 4 thử thách, 1 hồi quy nghiêm trọng. Đã sửa hành vi đúng mong đợi:
  - #1: `tra_cuu_don` chỉ trả về ngày nhận và trạng thái, không kiểm được tem mác → trợ lý nhắc khách giữ tem mác thay vì khẳng định "còn tem mác".
  - #2: ghi rõ lời gọi `tra_cuu_don(MS-1050)` và `tao_yeu_cau_doi_tra`, không hứa tiền về sớm hơn 3–5 ngày.
  - #6: tin không có mã đơn → chuyển nhân viên ngay kèm lý do và xin mã đơn hoặc số điện thoại, không đoán đơn (thêm CS-5), không từ chối vì quá 7 ngày.
  - #8: thêm bước tiếp theo sau khi từ chối hoàn tiền (hỏi hàng có lỗi không, có thì chuyển nhân viên) để tránh lỗi `no_next_step`.
