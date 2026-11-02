# Kế hoạch — Làm lại lab2 qua AI (sau crash course)

> Cho Claude và người dùng. Crash course V-01..V-15 đã xong (2026-11-02). Đây không phải khối V-xx mới: người dùng **tự làm** qua AI, Claude **hỗ trợ đọc và gọi tên lỗi**.
> **Cách viết:** theo `docs/07-communication-style.md` (D-020).
> **Figma lab2 chỉ đọc** (PRC-005). Bản làm lại nằm ở file Figma mới hoặc bản sao, hoặc HTML do AI dựng; không ghi đè file `1qIZVpL0Q7bD9UzT5TVBRy`.
> Nguồn: brief `docs/lab2-brief-gv001.md`, artifact V-15 (https://claude.ai/artifact/GfQN3phhfyg4Aw367dhYMx), màn cần làm trong `thiengthb/prm323-lab2-SE190533/design/screen-spec.md`.

## Câu hỏi đầu tiên cho người dùng (hỏi một lần, tối đa 3 câu)
1. Bật lại phê bình (PRC-004) không? Nếu bật: Claude chấm từng bản theo `templates/review-checklist.md` và ghi `log/critique-scores.md`. Nếu không: Claude chỉ trả lời checklist 15 câu kèm bằng chứng.
2. Làm bằng công cụ AI nào (Claude dựng HTML, Figma Make, v0…)? Quyết định định dạng đầu ra.
3. Đã chốt bảy quyết định trong artifact V-15 chưa? Chưa thì chốt trước bước 1.

## Thứ tự màn
Màn trước dạy màn sau, nên làm theo thứ tự từ màn bị chê nặng nhất:
1. **GV-001 Tổng quan**: màn thầy nhìn đầu tiên, bị lưới bốn ô số và gờ ở mọi thẻ (M0-01, lỗi lưới KPI và đồng phục). Brief đã có.
2. **GV-102 Phiên điểm danh**: lỗi switch để đánh dấu có mặt (M0-01, lỗi control sai nghĩa); hành động chính là Chốt. Viết brief mới bằng máy V-15: đổi phần Mục tiêu, Nội dung, Trạng thái.
3. **GV-104 Chú ý** và **GV-201 Hồ sơ sinh viên**: danh sách và chi tiết; dùng câu lệnh V-06, V-08, V-10.
4. Các màn còn lại (GV-002, GV-003, GV-101, GV-103, GV-105, GV-004, nhóm đăng nhập GV-09x): áp lại token và quyết định đã chốt, ít cần brief riêng.

## Vòng làm một màn
1. Ráp brief (máy V-15, hoặc sửa bản chữ trong `docs/`).
2. Dán cho AI, đòi ba hướng khác cấu trúc (câu lệnh V-15 số 2).
3. Người dùng chọn một hướng và ghi một câu vì sao.
4. AI làm chi tiết và các trạng thái (câu lệnh V-15 số 3, 5).
5. Soát bằng checklist 15 câu (AI tự soát kèm bằng chứng, rồi Claude soát lại).
6. Xem chuyển động ở tốc độ thật và 0,25× nếu có prototype (PRC-002).
7. Xuất token và quyết định (câu lệnh V-15 số 6), cập nhật DESIGN.md của lab2 khi người dùng đồng ý.

## Lưu vào repo này sau mỗi màn
- Ảnh hoặc file kết quả trong `demos/LAB2/<mã màn>/`.
- Brief màn đó trong `docs/lab2-brief-<mã màn>.md`.
- Luật mới rút ra (draft) vào `rules/`, người dùng duyệt mới thành adopted.
- PROGRESS, SESSIONS, push, đồng bộ `log/PROGRESS.md` sang Project claude.ai.

## Khi nào mang cho thầy
Sau khi GV-001 và GV-102 qua checklist 15 câu. Mỗi quyết định lớn chuẩn bị một câu "vì sao" bằng tên gọi đã học (để tránh tình huống thầy hỏi "vì sao nút cao 48dp?" mà không trả lời được, M0-01 mục 8).
