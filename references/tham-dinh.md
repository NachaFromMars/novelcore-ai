# Thẩm Định — Prompt & Quy Trình Chi Tiết

## Prompt Thẩm Định Đơn Bản

```
Đọc beat dưới đây. Chấm điểm 7 tiêu chí, mỗi tiêu chí cho điểm riêng từ 1 đến 10, kèm lý do cụ thể 1 đến 2 câu. Sau đó tính tổng có trọng số.

Nếu dưới 9/10: chỉ ra đúng 3 điểm yếu nhất, mỗi điểm kèm gợi ý sửa cụ thể (chỉ vị trí, chỉ hướng, không viết thay).
Nếu đạt 9/10 trở lên: ghi PASS.

7 tiêu chí và trọng số:
1. Giọng văn đúng nhân vật, đúng tone dự án (20%)
2. Nhịp văn: tempo, câu dài ngắn xen kẽ (15%)
3. Cảm xúc đạt mục tiêu beat (15%)
4. Không dấu vết AI: từ sáo, cấu trúc lặp (15%)
5. Đối thoại tự nhiên, có cá tính (15%)
6. Show don't tell (10%)
7. Nối mạch với beat trước và sau (10%)

Chấm khắt khe. Điểm 8 là đã rất tốt. Điểm 9 là mức xuất bản. Điểm 10 gần như không tồn tại.

Ngữ cảnh: [paste 1-2 đoạn cuối beat trước]
Mục tiêu beat: [ghi rõ cảm xúc, hành động, điểm nối]
Beat cần thẩm định:
[paste beat]
```

## Prompt So Sánh Ba Bản

```
Dưới đây là 3 bản viết cho cùng một beat.
So sánh cả 3 theo 7 tiêu chí trên. Chấm điểm từng bản riêng. Chọn bản tốt nhất, giải thích tại sao bản đó thắng.
Nếu không bản nào đạt 9/10, chỉ ra bản nào gần nhất và cần sửa gì.
Chấm khắt khe. Tìm ít nhất 3 điểm yếu mỗi bản, bất kể bài viết hay cỡ nào.

Bản A: [paste]
Bản B: [paste]
Bản C: [paste]
```

## Chống Lạm Phát Điểm — 4 Kỹ Thuật

1. **Neo thang điểm** — Thêm: "Chấm khắt khe. 8 = rất tốt. 9 = mức xuất bản. 10 = gần như không tồn tại."
2. **Ép tìm điểm yếu** — "Tìm ít nhất 5 điểm yếu bất kể hay cỡ nào." AI không tìm đủ 5 = đang lười, không phải bài viết hoàn hảo.
3. **So sánh chuẩn** — "So sánh beat với prose cấp độ xuất bản thương mại tiếng Việt. Chỉ ra khoảng cách."
4. **Cross-check ngược** — Sau khi AI chấm 9/10: "Đóng vai biên tập viên khắt khe nhất. Tìm mọi lý do hạ điểm." Nếu tìm >3 lý do hợp lệ → điểm 9 là giả.

**Quy tắc sống còn:** AI cho 10/10 = gần như chắc chắn đang nịnh.
