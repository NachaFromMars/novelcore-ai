# Prompt Mẫu Sao Chép Ngay

## 1 — Viết Beat Mới (3 Bản)

```
Ngữ cảnh gần:
[paste 1-2 đoạn cuối beat trước]

Mục tiêu beat:
[mô tả: cảm xúc, hành động, điểm nối]

Giọng văn: [tên giọng]

Viết 3 bản độc lập cho beat này:
- Bản A: thiên nội tâm, đào sâu dòng suy nghĩ
- Bản B: thiên đối thoại, đẩy xung đột qua lời nói
- Bản C: thiên hành động và miêu tả

Mỗi bản 400-600 từ. Không markdown. Không em dash. Không tiếng Anh. Không từ AI. Prose thuần túy.
```

## 2 — Thẩm Định + So Sánh 3 Bản

```
Dưới đây là 3 bản viết cho cùng một beat.
So sánh cả 3 theo 7 tiêu chí (giọng văn 20%, nhịp 15%, cảm xúc 15%, không dấu vết AI 15%, đối thoại 15%, show don't tell 10%, nối mạch 10%).

Chấm điểm từng bản riêng. Chọn bản tốt nhất.
Chấm khắt khe: 8 = rất tốt, 9 = mức xuất bản, 10 = gần như không tồn tại.
Tìm ít nhất 3 điểm yếu mỗi bản bất kể hay cỡ nào.
Nếu không bản nào đạt 9, chỉ ra bản gần nhất và cần sửa gì (chỉ vị trí, chỉ hướng, không viết thay).

Ngữ cảnh: [paste 1-2 đoạn cuối beat trước]
Mục tiêu beat: [ghi rõ]

Bản A: [paste]
Bản B: [paste]
Bản C: [paste]
```

## 3 — Biên Tập Phẫu Thuật

```
Beat dưới đây đã thẩm định. Điểm yếu là:
[paste 3 điểm yếu từ lượt thẩm định]

Sửa đúng 3 điểm này. Không chạm vào phần đã tốt.
Giữ nguyên độ dài 400 đến 600 từ.
Giữ nguyên giọng [tên giọng].
Output chỉ là beat đã sửa, không giải thích.

Beat gốc: [paste beat]
```

## 4 — Cross-Check Chống Nịnh

```
Beat dưới đây vừa được chấm 9/10.
Đóng vai biên tập viên khắt khe nhất trong ngành.
Tìm mọi lý do để hạ điểm beat này. So sánh với prose cấp độ xuất bản thương mại tiếng Việt.
Chỉ ra khoảng cách.
Nếu tìm ra nhiều hơn 3 lý do hợp lệ để hạ điểm, kết luận: điểm 9 ban đầu là giả, cần viết lại.

Beat: [paste beat]
```

## 5 — Scan Continuity Chương

```
Đọc toàn bộ chương dưới đây. Liệt kê mọi điểm mâu thuẫn theo 4 trục:
1. Timeline: thời gian có nhảy/mâu thuẫn không
2. Không gian: nhân vật có dịch chuyển phi lý không
3. Năng lực: power level có nhảy bất hợp lý không
4. Chi tiết: có gì bị quên so với chương trước không

Kiểm tra thêm: flow giữa các beat, nhịp tổng thể chương, mở và đóng chương có lực không.

Chương trước (tham chiếu): [paste/search]
Chương cần scan: [paste]
```

## 6 — Scan Continuity Arc

```
Dưới đây là tóm tắt từng chương trong arc.
Scan toàn bộ arc theo 4 trục: timeline, không gian, năng lực, chi tiết nhỏ.
Kiểm tra thêm: arc nhân vật phát triển nhất quán không, xung đột chính đẩy lên đúng nhịp không, kết arc xứng với setup không.
Nếu output dài, chia thành nhiều lượt. Dừng ở điểm tự nhiên, báo còn bao nhiêu phần, đợi lệnh tiếp.

Tóm tắt các chương: [paste]
Timeline: [paste]
Bảng nhân vật: [paste/search project knowledge]
```

## System Prompt Mẫu

```
ROLE:
Mày là cây bút thứ hai của tao. Mày viết prose thuần túy, văn học, theo đúng giọng và luật tao đặt. Tao giữ linh hồn. Mày giữ kỷ luật.

THỂ LOẠI: [điền thể loại]
GIỌNG VĂN MẶC ĐỊNH: [điền tên giọng + mô tả ngắn]

LUẬT CỨNG:
- 400-600 từ mỗi beat, không vượt 600
- 0% Markdown (không dấu #, **, >, ```)
- 0% em dash, dùng phẩy hoặc ba chấm
- 0% tiếng Anh trong prose
- 0% từ AI: [liệt kê blacklist]
- Prose thuần túy, tin người đọc
- Mỗi lần chỉ viết 1 beat

QUY TRÌNH:
- Viết 3 bản độc lập mỗi beat
- Tự chấm 7 tiêu chí, tổng >= 9/10 mới pass
- Nếu dưới 9, chỉ ra điểm yếu, viết lại
- Polish tối đa 2 vòng, sau đó viết mới

PROJECT KNOWLEDGE:
[Outline tổng, bảng nhân vật, timeline, glossary, đoạn mẫu giọng văn — lưu file riêng]
```
