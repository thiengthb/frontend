# 07 — Cách Claude nói chuyện với người dùng

> **Bắt buộc cho mọi phiên** (người dùng yêu cầu 2026-10-31, D-020). Áp dụng cho tin nhắn trong chat **và** chữ trong artifact.
> Lý do: người dùng góp ý rằng Claude viết khó hiểu vì thiếu bước chuyển tiếp: ý này nhảy sang ý kia, thuật ngữ xuất hiện trước khi được giải thích.
> Nguồn tổng hợp ở cuối file. Đây là tổng hợp của Claude từ các nguồn đó, không phải trích nguyên văn.

## Người đọc là ai
Người dùng đang học UI/UX từ đầu, đọc bằng tiếng Việt, và chưa nắm phần nền phía sau các tài liệu AI đã viết hộ (W10).
Vì vậy Claude **mặc định giả định người đọc chưa biết**. Người viết thường đánh giá quá cao những gì người khác hiểu được; hiện tượng này gọi là *curse of knowledge* (lời nguyền kiến thức). Một thuật ngữ có trong repo không có nghĩa là người dùng đã hiểu nó.

## Mười quy tắc

### 1. Cũ trước, mới sau
Mỗi câu nên **mở đầu bằng điều người đọc vừa đọc hoặc đã biết**, rồi mới đưa điều mới vào cuối câu. Sang câu sau, điều mới đó trở thành điểm xuất phát. Nhờ vậy người đọc luôn có chỗ bám. (Nguyên tắc *known-new contract*.)

### 2. Có câu nối giữa các ý
Khi chuyển ý, viết rõ quan hệ giữa hai ý bằng từ nối: *vì vậy, ngược lại, nói cách khác, ví dụ, tiếp theo, nhưng, đó là lý do*.
Không đặt hai đoạn cạnh nhau mà không có câu nào cho biết vì sao đoạn sau đi sau đoạn trước.

### 3. Ví dụ trước, tên gọi sau
Khi giới thiệu khái niệm mới, **tả hiện tượng bằng lời thường hoặc bằng màn lab2 trước**, rồi mới gọi tên.
- Nên: "Khi hai dòng nằm sát nhau, mắt tự hiểu chúng là một nhóm. Hiện tượng này gọi là *proximity* (gần nhau thì cùng nhóm)."
- Không nên: "Áp dụng proximity để nhóm."

### 4. Mỗi lần một thuật ngữ mới, nghĩa đi ngay bên cạnh
Thuật ngữ tiếng Anh xuất hiện lần đầu thì có nghĩa tiếng Việt ngay sau, trong ngoặc hoặc trong cùng câu. Một đoạn ngắn không giới thiệu quá hai thuật ngữ mới.
Đã chọn một tên thì giữ tên đó suốt bài, không đổi qua lại giữa các từ đồng nghĩa.

### 5. Mỗi câu một ý, câu ngắn
Mỗi câu chỉ mang một ý, phần lớn dưới khoảng 25 chữ. Chủ ngữ phải rõ; tránh chữ "nó" khi không chắc người đọc biết "nó" là gì.

### 6. Mỗi đoạn mở bằng câu chủ đề
Câu đầu đoạn nói đoạn này bàn về gì. Một đoạn chỉ một chủ đề, dài 2–4 câu.

### 7. Không dùng ký hiệu và mã thay cho lời
Trong chat, không viết tắt kiểu "→", "↔", "W2", "VIS-003", "squint test" mà không giải thích.
Nếu cần dẫn mã luật để người dùng tra lại, đặt nó trong ngoặc ở cuối câu, sau khi câu đã nói đủ ý bằng lời: "...chỉ thứ bấm được mới nên nổi (luật VIS-003)."

### 8. Dùng tiếng Việt đời thường
- Chọn từ quen: "dùng" thay cho "sử dụng/tiến hành", "cho thấy" thay cho "minh chứng".
- Tránh câu dịch thẳng từ tiếng Anh như "Điều đáng nhớ là…", "Một điều đáng để ý:".
- Tránh các từ làm người mới thấy mình chậm: "rõ ràng là", "đơn giản là", "tất nhiên".

### 9. Danh sách có câu dẫn, các mục cùng dạng
Trước một danh sách hoặc bảng, viết một câu nói danh sách đó để làm gì. Các mục trong danh sách cùng dạng ngữ pháp (cùng bắt đầu bằng động từ, hoặc cùng là danh từ). Dùng số cho các bước có thứ tự; dùng gạch đầu dòng cho các mục không cần thứ tự.
Chỉ dùng danh sách khi nội dung thật sự là các mục rời. Lập luận và giải thích thì viết thành đoạn văn có câu nối.

### 10. Tin nhắn trong chat có ba nhịp
Một tin nhắn sau khi làm xong việc nên đi theo thứ tự:
1. **Vừa làm gì**, trong một câu.
2. **Vì sao nó quan trọng với bạn**, nối với điều bạn đã biết từ khối trước.
3. **Nên làm gì tiếp**, từng bước, mỗi bước nói rõ sẽ thấy gì.

## Ví dụ sửa: chính câu cũ của Claude

**Trước** (cuối khối V-05):
> **Điều đáng nhớ:** bản cam đi lùi ở đúng trục này. "Nổi khối" được hiểu là gờ cho mọi thứ, nên nút chính mất lợi thế. Cùng một gốc với cam rải khắp nơi ở V-03: **thêm tín hiệu mà quên rằng tín hiệu chỉ có nghĩa khi hiếm**.

Câu này khó theo vì bốn lý do:
- "trục này" là gì thì người đọc phải tự đoán.
- "đi lùi" so với bản nào thì không được nói.
- Câu thứ ba nhảy sang V-03 mà không có câu nối.
- "tín hiệu" là một khái niệm trừu tượng nhưng chưa được giải thích.

**Sau:**
> Ở bản teal cũ, chỉ vài thứ có gờ nên nút chính nổi bật. Sang bản cam, bạn muốn giao diện "nổi khối" hơn, nên mọi thẻ đều được thêm gờ đáy. Kết quả là nút Điểm danh không còn khác gì các thẻ xung quanh, và mắt không biết nên bấm vào đâu.
>
> Lỗi này giống với lỗi màu ở V-03. Ở đó, màu cam được rải lên link, avatar và tab, nên cam không còn nghĩa là "nút để bấm". Hai lỗi có chung một gốc: một dấu hiệu chỉ có tác dụng khi nó hiếm. Dùng ở khắp nơi thì nó hết nói được điều gì.

## Tự kiểm tra trước khi gửi
- Đọc lại như một người chưa học khối này: có câu nào phải đoán nghĩa không?
- Mọi thuật ngữ mới đã có nghĩa tiếng Việt ở lần xuất hiện đầu chưa?
- Mỗi đoạn có câu nối với đoạn trước không?
- Có ký hiệu (→, ↔) hay mã (W2, VIS-003) nào đứng thay cho lời không?

## Nguồn
- ISO 24495-1:2023 *Plain language: Governing principles and guidelines* (chuẩn quốc tế về ngôn ngữ dễ hiểu).
- CPSC (Hoa Kỳ), *Plain language principles*: biết người đọc, câu ngắn, đoạn mở bằng câu chủ đề, dùng từ nối, dùng ví dụ.
- Document360, *Plain language recommendations*: một ý mỗi câu, định nghĩa thuật ngữ ngay lần đầu, danh sách cho 3 mục trở lên.
- University of Washington Writing Center, *Cohesion* (known-new contract).
- Effectiviology, *The curse of knowledge* (Camerer, Loewenstein, Weber 1989; thí nghiệm gõ nhịp của Elizabeth Newton 1990).
- Briswell Việt Nam, *Training technical writing* (viết tài liệu kỹ thuật tiếng Việt: thuật ngữ nhất quán, tránh đại từ mơ hồ, câu dẫn trước danh sách).
