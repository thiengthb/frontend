# PROGRESS — Nguồn sự thật về tiến độ

> Cập nhật cuối mỗi phiên. Phiên Claude mới đọc file này đầu tiên.

## Trạng thái hiện tại
- **Ngày cập nhật:** 2026-10-30
- **Module:** M0 — Chẩn đoán. **M0-01 xong** (`lessons/M0-01-baseline.md`), đang chờ người dùng phản biện
- **Lộ trình:** v2 (`docs/02-roadmap.md`), 13 module, nhịp 4 giờ/tuần, khoảng 12 tháng
- **Luật hiện có (đều draft):** VIS-001..003, UX-001, CMP-001, PRC-001..003, COL-001

## Kết luận chẩn đoán (tóm tắt cho phiên sau)
Mạnh về hệ thống, trạng thái, a11y và tooling. Yếu ở **phân cấp cấp trang, tương phản tỉ lệ, cá tính, chuyển động**.
Gốc rễ (W1) là tối ưu cho "không sai" thay vì "hay". Thêm W2: nhất quán bị hiểu thành đồng phục.

## Bước tiếp theo
1. Người dùng **phản biện M0-01** (đồng ý hoặc không với W1–W9) và trả lời 3 câu hỏi mở cuối bài.
2. Người dùng làm **BT-M0-01 "Ba bố cục, không đổi màu"** cho lab2 GV-001, bằng tay, không AI.
3. Buổi sau: review BT-M0-01, rồi **M0-02 Moodboard gu**, rồi vào **M1-01 Visual hierarchy**.

## Câu hỏi còn mở
- Thầy nhận xét "đơn điệu" trên bản cam (Figma hiện tại) hay bản teal (ảnh trong repo lab2)?
- Lỗi spring `[object Object]` trong `thienui/apps/docs/registry/lib/motion-tokens.ts`: người dùng tự sửa (bài tập M9-05) hay Claude mở PR?
- Người dùng có muốn duyệt (chuyển `adopted`) luật nào từ M0-01 ngay không?

## Bối cảnh người dùng
- Thiết kế chủ yếu qua AI (duyệt và yêu cầu sửa); từng làm Figma bằng tay một lần. Stack: React, Vite, Next.js
- 4 giờ/tuần
