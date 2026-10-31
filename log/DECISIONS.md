# DECISIONS — Các quyết định đã chốt

> Chỉ thêm, không xoá. Muốn đảo một quyết định thì thêm mục mới tham chiếu mục cũ.

| # | Ngày | Quyết định | Lý do | Ai chốt |
|---|---|---|---|---|
| D-001 | 2026-10-30 | Ngôn ngữ làm việc là tiếng Việt, thuật ngữ giữ tiếng Anh | Người dùng cần gọi tên chính xác khi ra đề cho AI | người dùng + Claude |
| D-002 | 2026-10-30 | Mọi luật phải có Loại, Lý do, Trạng thái; chỉ người dùng được chuyển sang `adopted` | Tránh bộ luật phình to, mâu thuẫn, thiếu cơ sở | Claude đề xuất |
| D-003 | 2026-10-30 | Git repo là nguồn sự thật; chat chỉ là nơi làm việc | Cho phép nhiều tài khoản/phiên Claude tiếp nối mà không lệch | Claude đề xuất |
| D-004 | 2026-10-30 | Nhịp học 4 giờ/tuần, khoảng 1 bài/tuần; lộ trình v2 khoảng 12 tháng | Người dùng cho biết quỹ thời gian | người dùng |
| D-005 | 2026-10-30 | Claude đóng vai người phê bình khắt khe, không chiều lòng (CLAUDE.md mục 4a) | Người dùng yêu cầu "đập đi đập lại" | người dùng |
| D-006 | 2026-10-30 | Thêm M5 tâm lý hành vi, M6 nghiên cứu người dùng, M7 quy chuẩn & tỉ lệ, M9 Animation riêng | Người dùng yêu cầu | người dùng |
| D-007 | 2026-10-30 | Repo `thiengthb/frontend` là nơi chứa playbook (thay cho zip) | Người dùng tạo repo | người dùng |
| D-008 | 2026-10-30 | Học dồn bằng crash course 3 ngày trước, rồi làm lại lab2; lộ trình 12 tháng thành deep track | Người dùng muốn áp dụng nhanh vào lab2 | người dùng |
| D-009 | 2026-10-30 | Critique Loop: subagent làm bài, người dùng phê bình, Claude chấm cả hai (PRC-004); PRC-003 deprecated | Người dùng đề xuất; luyện đúng kỹ năng art-direct AI | người dùng (Claude thêm bước dự đoán, chờ duyệt) |
| D-010 | 2026-10-30 | Ưu tiên tài liệu video, link phải được kiểm là có tồn tại, đánh dấu ⚠ nếu chưa rõ chất lượng | Người dùng học trực quan | người dùng |
| D-011 | 2026-10-30 | Duyệt PRC-004 kèm bước dự đoán 2 phút | Người dùng đồng ý | người dùng |
| D-012 | 2026-10-30 | Mỗi Mốc một chat mới (PRC-006); Claude chủ động đề xuất cải tiến cách học | Tránh ngữ cảnh quá dài | người dùng |
| D-013 | 2026-10-30 | Figma của người dùng mặc định chỉ đọc (PRC-005, draft) | Phiên trước đã làm hỏng file lab2 | Claude đề xuất |
| D-014 | 2026-10-30 | Sửa D-012: mỗi **khối** CC-xx một chat (không phải mỗi Mốc); chat kết thúc phải viết sẵn brief khối sau | Người dùng làm rõ | người dùng |
| D-015 | 2026-10-31 | Duyệt VIS-004, VIS-005, UX-002 sang `adopted` | Rút từ CC-01; người dùng đồng ý | người dùng |
| D-016 | 2026-10-31 | CC-01 được 3/10 (< 4) nhưng **không làm lại cả khối**: mở đầu CC-02 bằng 5 phút phê bình lại một khung của CC-01, bắt buộc dùng thuật ngữ và hướng sửa | Mục tiêu khối 1 vốn là 3–4/10; chỗ yếu là ngôn ngữ và hướng sửa, không phải mắt; người dùng thiếu thời gian | Claude đề xuất, người dùng có thể bác ở đầu CC-02 |
| D-017 | 2026-10-31 | Khi thiếu thời gian, người dùng được thay video bằng bản tóm tắt của Claude và bỏ bước dự đoán | Người dùng yêu cầu ở CC-01 | người dùng |
| D-018 | 2026-10-31 | Thiết kế lại crash course thành **trực quan, chỉ đọc và nghịch** (`docs/05-crash-course.md` v2, 15 khối V-01..V-15, PRC-007). Bỏ bài tập, chấm điểm, quiz đầu khối; PRC-004 tạm ngưng tới lab2. Mỗi khối có câu lệnh mẫu cho AI, cộng dồn vào `docs/06-ai-prompt-dictionary.md` | Người dùng đang ở tầng nhớ và nhận diện, cần đi nhanh và liên tục; làm bài tốn năng lượng. Claude nêu rủi ro ảo giác năng lực (W10), người dùng chấp nhận; bù bằng lab2 | người dùng |
| D-019 | 2026-10-31 | Sửa PRC-006: một chat làm liên tiếp 2–3 khối V-xx, mở chat mới khi dài; bàn giao bằng PROGRESS + brief khối kế | Học liên tục, ít ma sát mở chat | Claude đề xuất theo yêu cầu "đi nhanh, liên tục" của người dùng |
| D-020 | 2026-10-31 | Claude viết theo `docs/07-communication-style.md` (tiếng Việt dễ hiểu, có bước chuyển tiếp) cho cả chat và artifact; CLAUDE.md §2, §4 trỏ tới file này | Người dùng góp ý cách truyền đạt khó hiểu vì thiếu câu nối, thuật ngữ đến trước giải thích; yêu cầu tra nguồn về cách viết dễ hiểu | người dùng |
