# PROGRESS — Nguồn sự thật về tiến độ

> Cập nhật cuối mỗi phiên. Phiên Claude mới đọc file này đầu tiên.

## Trạng thái hiện tại
- **Ngày cập nhật:** 2026-11-01
- **Chế độ:** **Crash course TRỰC QUAN v2** (`docs/05-crash-course.md`, D-018, PRC-007): mỗi khối V-xx là một artifact tương tác Claude dựng sẵn; người dùng chỉ đọc và nghịch. **Không bài tập, không chấm, không quiz đầu khối.**
- **Đã học theo cách cũ (v1):** CC-01 phân cấp (xong), nửa đầu CC-02 typography (bài giảng + demo inline). Tài liệu tái dùng cho V-01, V-02.
- **Đã xong (v2):** **V-01 Phân cấp & điểm nhấn** (2026-10-31): `demos/V-01/hierarchy.html`, artifact "V-01 Phân cấp" (https://claude.ai/artifact/UUdsaDzKfNx3L3FchPDvf6).
- **Đã xong (v2):** **V-02 Typography** (2026-10-31): `demos/V-02/typography.html`, artifact "V-02 Typography" (https://claude.ai/artifact/Bno3KC7pqjaFWUhq1TRWtR).
- **Đã xong (v2):** **V-03 Màu** (2026-10-31): `demos/V-03/color.html`, artifact "V-03 Màu" (https://claude.ai/artifact/2v5aB6144b1NQLVfwagqr8).
- **Đã xong (v2):** **V-04 Khoảng cách, lưới, nhịp** (2026-10-31): `demos/V-04/spacing.html`, artifact "V-04 Khoảng cách" (https://claude.ai/artifact/KGywbwkZMX8xFHQVYe3rXW).
- **Đã xong (v2):** **V-05 Chiều sâu & hình khối** (2026-10-31): `demos/V-05/depth.html`, artifact "V-05 Chiều sâu" (https://claude.ai/artifact/5Y7Mfy4v46H5zAPk8fJiJN). **Hết Ngày 1 · NHÌN.**
- **Đã xong (v2):** **V-06 Bố cục màn mobile** (2026-10-31): `demos/V-06/layouts.html`, artifact "V-06 Bố cục mobile" (https://claude.ai/artifact/DGMcrKEfwBinoTshtD9hhA). Mở đầu Ngày 2 · PATTERN. Viết theo D-020.
- **Đã xong (v2):** **V-07 Nút & điều khiển** (2026-10-31): `demos/V-07/controls.html`, artifact "V-07 Nút & điều khiển" (https://claude.ai/artifact/HzziX3fF9nDyDw2B4WaZmT).
- **Đã xong (v2):** **V-08 Điều hướng & kiến trúc thông tin** (2026-11-01): `demos/V-08/navigation.html`, artifact "V-08 Điều hướng" (https://claude.ai/artifact/4vcSrpMqk2CZ4C6n4epvKa).
- **Đã xong (v2):** **V-09 Trạng thái & phản hồi** (2026-11-01): `demos/V-09/states.html`, artifact "V-09 Trạng thái" (https://claude.ai/artifact/38ZdD6wwdfebeFhT4UNW6T).
- **Đã xong (v2):** **V-10 Định luật UX bằng hình** (2026-11-01): `demos/V-10/laws.html`, artifact "V-10 Định luật UX" (https://claude.ai/artifact/Sf2VdJPWUVJnNh3A35acK3). **Hết Ngày 2 · PATTERN.**
- **Đã xong (v2):** **V-11 Trợ năng bằng con số** (2026-11-01): `demos/V-11/a11y.html`, artifact "V-11 Trợ năng" (https://claude.ai/artifact/KUmnnNWvuFJGNrvLL4CaZm). Mở đầu Ngày 3.
- **Đã xong (v2):** **V-12 Chuyển động 1** (2026-11-01): `demos/V-12/motion.html`, artifact "V-12 Chuyển động" (https://claude.ai/artifact/XgWXmu8R1z9wB45F3virwU).
- **Cách viết mới (D-020):** từ V-06, chat và artifact theo `docs/07-communication-style.md`. Có thể sửa lại chữ V-01..V-05 theo chuẩn này nếu người dùng muốn.
- **Khối tiếp theo:** **V-13 Chuyển động 2** (brief: `docs/briefs/V-13.md`). Chat này đã làm V-11, V-12: làm V-13 xong thì **mở chat mới** (PRC-006).
- **Luật:** adopted: PRC-004 (tạm ngưng), PRC-006 (sửa D-019), PRC-007, VIS-004, VIS-005, UX-002. Draft: VIS-001..003, UX-001, CMP-001, COL-001, PRC-001, 002, 005. Deprecated: PRC-003
- **Từ điển ra lệnh AI:** `docs/06-ai-prompt-dictionary.md` (đã có V-01..V-12; mỗi mục 6 câu)

## Bước tiếp theo
**Tiếp:** dựng **V-13** theo `docs/briefs/V-13.md` (load `artifact-design`, tái dùng khung `demos/V-12/motion.html`, kiểm nguồn spring trước khi ghi số, đọc mã spring của thienui, publish "V-13 Chuyển động 2") → giải thích ≤ 10 dòng theo ba nhịp. Nếu chat mới: clone → đọc file này → tóm tắt ≤ 2 dòng → dựng ngay.
Cuối mỗi khối: `demos/V-xx/`, từ điển, glossary, brief khối kế, PROGRESS, push. Sau khi push, đồng bộ `log/PROGRESS.md` sang Project claude.ai (bản Project hay bị cũ).

## Câu hỏi còn mở
- Lab2 có nút cao 40 (trong thẻ) và 36 (trong hộp thoại): khi làm lại, ghi rõ vùng chạm vô hình mở rộng tới 48 hay chấp nhận dưới 48 (V-11, mục Trên lab2).
- Lỗi spring `[object Object]` trong thienui: minh hoạ ở V-13.
- Ba câu IA còn mập mờ của lab2 (ghi ở V-08, mục Trên lab2): yêu cầu sửa điểm danh ở Tổng quan hay Lớp; màn Điểm danh hai lối vào thì ‹ về đâu; chạm em sinh viên ở Tổng quan thì mở trong ngăn xếp Tổng quan hay nhảy sang Lớp. Người dùng tự chọn khi làm lại lab2.
- Hai quyết định trạng thái cho lab2 (ghi ở V-09): GV-001 .X nên giữ dữ liệu cũ kèm dải báo thay vì thay cả màn (Claude đề xuất); nút Chốt có cả hộp xác nhận lẫn Hoàn tác, giữ hay bỏ hộp. Thêm gợi ý tự gửi lại khi có mạng và empty state "đã xử lý hết" cho GV-105.

## Bối cảnh người dùng
- Thiết kế chủ yếu qua AI; chưa hiểu nền tảng sau các artefact AI làm hộ (W10)
- Giai đoạn hiện tại: **học vẹt, biết và hiểu sơ** để nhận diện pattern, thuật ngữ, và ra lệnh cho AI; muốn học trực quan, đọc nhanh, liên tục, ít tốn năng lượng
- Stack: React, Vite, Next.js. Học dồn 2–3 ngày, sau đó 4 giờ/tuần
- Mục tiêu gần: làm lại lab2 (thầy chê bản cam là đơn điệu)
