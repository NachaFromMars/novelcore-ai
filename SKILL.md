---
name: novelcore-ai
description: "NovelCoreAI V2.0 — Quy trình viết tiểu thuyết với AI, từ ý tưởng đến bản thảo hoàn chỉnh. Dùng khi: (1) viết novel/tiểu thuyết dài với AI, (2) forge beat/chương tiểu thuyết, (3) thẩm định chất lượng prose, (4) biên tập phẫu thuật beat, (5) scan continuity chương/arc, (6) chống lạm phát điểm AI, (7) quản lý token budget và context phân vùng cho novel. Triggers: novel, tiểu thuyết, viết chương, forge beat, thẩm định beat, biên tập prose, scan continuity, novelcore, chấm điểm beat, prose quality, fiction writing."
---

# NovelCoreAI V2.0 — Premium Blueprint

Quy trình viết tiểu thuyết với AI. Nền tảng V1.0 của tác giả, nâng cấp bởi Claude Opus 4.6.

## Triết Lý Cốt Lõi

- AI là cây bút thứ hai, không viết thay tác giả. Tác giả giữ linh hồn, giọng văn, tầm nhìn. AI giữ kỷ luật, tốc độ, biến thể.
- **Viết ít, viết chậm, viết đúng.** Chất lượng từng beat quyết định chất lượng cả cuốn sách.
- **Tách sáng tạo và phê bình.** Không bắt AI vừa viết vừa thẩm định cùng lượt. Trộn lẫn thì cả hai đều yếu.
- **Prompt cụ thể sinh output cụ thể.** Prompt mơ hồ sinh output mơ hồ.

## Thông Số Kỹ Thuật Tối Ưu

| Thông số | Giá trị | Giải thích |
|---|---|---|
| Token mỗi lần viết | 800-1500 | Vùng vàng chất lượng prose tiếng Việt |
| Từ tiếng Việt mỗi beat | 400-600 | Tuyệt đối không vượt 600 |
| Đơn vị mỗi lần prompt | 1 beat | Không bao giờ viết 2+ beat cùng lúc |

## Cấu Trúc Prompt Bốn Khối

Mỗi prompt viết prose gồm 4 khối:
1. **Bối cảnh** — AI đang ở đâu trong truyện (chương, beat, tình huống)
2. **Nhiệm vụ** — Beat phải đạt được gì (hành động, nội tâm, xung đột)
3. **Cảm xúc/Giọng văn** — Tone, atmosphere, tên giọng văn
4. **Ràng buộc kỹ thuật** — 400-600 từ, 0% markdown, 0% em dash, 0% tiếng Anh, 0% từ AI, prose thuần túy

Không nhồi lore dump vào prompt. Nếu cần backstory, tách file riêng trong project knowledge.

## Quy Trình Sáu Pha (Mỗi Chương)

1. **Kiến Trúc Chương** — Xác định mục tiêu arc, nhân vật thay đổi, xung đột. Prompt AI câu hỏi chiến lược, không phải câu hỏi viết.
2. **Outline Beat** — 5-8 beat/chương, mỗi beat có mục tiêu cảm xúc + hành động + điểm nối. Tác giả và AI cùng làm, tác giả duyệt cuối.
3. **Viết Ba Phiên Bản** — Mỗi beat viết 3 bản độc lập: A (nội tâm), B (đối thoại), C (hành động/miêu tả). Ba bản ép AI phá pattern.
4. **Thẩm Định** — AI chấm 7 tiêu chí, tổng ≥9/10 mới pass. Xem [references/tham-dinh.md](references/tham-dinh.md).
5. **Polish Có Mục Tiêu** — Chỉ đích danh 2-3 điểm cần sửa, không "viết lại cho hay hơn". Tối đa 2 vòng, sau đó viết mới.
6. **Scan Liên Tục** — Scan continuity: timeline, vị trí, power level, chi tiết nhỏ.

## 7 Tiêu Chí Thẩm Định (Trọng Số)

| Tiêu chí | Trọng số |
|---|---|
| Giọng văn nhất quán với nhân vật POV | 20% |
| Nhịp văn (tempo, câu dài ngắn xen kẽ) | 15% |
| Cảm xúc đạt mục tiêu beat | 15% |
| Không dấu vết AI (từ sáo, cấu trúc lặp) | 15% |
| Đối thoại tự nhiên, có cá tính | 15% |
| Show don't tell | 10% |
| Nối mạch beat trước và sau | 10% |

Thang điểm: 8 = rất tốt, 9 = mức xuất bản, 10 = gần như không tồn tại.

## 7 Kỹ Thuật Cường Hoá

1. **Nạp ngữ cảnh gần** — Paste 1-2 đoạn cuối chương/beat cũ trước khi viết mới
2. **Đặt tên giọng văn** — Mỗi nhân vật POV có tên giọng riêng + đoạn mẫu 100 từ
3. **Feedback phẫu thuật** — Chỉ đích danh vị trí + hướng sửa, không nói chung chung
4. **Project Knowledge** — Lưu outline, bảng nhân vật, timeline, glossary, bản đồ
5. **Blacklist từ cấm** — Liệt kê từ/cụm từ AI hay dùng mà ghét
6. **Viết ngược** — Prompt AI viết câu cuối trước rồi xây ngược lên
7. **Chia lượt dài** — Output dài chia nhiều lượt, dừng điểm tự nhiên

## Token Budget Tối Ưu

| Tác vụ | Output tối ưu |
|---|---|
| Viết 1 beat | 400-600 từ |
| Thẩm định 1 beat | 800-1200 từ |
| So sánh 3 bản | 1500-2000 từ |
| Biên tập/sửa beat | 400-600 từ |
| Scan continuity chương | 1000-1500 từ |
| Scan continuity arc | 2000-3000 từ (chia lượt) |

## Chống Lạm Phát Điểm

1. **Neo thang điểm** — "Chấm khắt khe. 8 = rất tốt, 9 = xuất bản, 10 = không tồn tại"
2. **Ép tìm điểm yếu** — "Tìm ít nhất 5 điểm yếu bất kể hay cỡ nào"
3. **So sánh chuẩn** — "So với prose xuất bản thương mại tiếng Việt, chỉ khoảng cách"
4. **Cross-check ngược** — Sau 9/10, bảo AI "đóng vai biên tập viên khắt khe nhất, tìm mọi lý do hạ điểm"

Nếu AI cho 10/10, gần như chắc chắn đang nịnh.

## Context Phân Vùng

| Tác vụ | Context cần nạp | Context KHÔNG nạp |
|---|---|---|
| Viết beat mới | 1-2 đoạn cuối beat trước + mục tiêu + giọng | Outline arc, backstory, lore dump |
| Thẩm định | Beat + ngữ cảnh gần + mục tiêu | Outline arc, beat khác |
| Biên tập | Beat gốc + 3 điểm yếu + tên giọng | Beat trước, outline |
| Scan chương | Toàn bộ chương + chương trước | Outline arc |
| Scan arc | Tóm tắt mỗi chương + timeline + bảng nhân vật | Full text mỗi chương |

## Workflow Tổng: Arc → EPUB

1. **Arc Blueprint** — Outline arc, mục tiêu chương, arc nhân vật, điểm ngoặt
2. **Chapter Outline** — 5-8 beat/chương, tác giả duyệt trước khi viết
3. **Beat Production** — Pha 3→5 cho từng beat: viết 3 bản → thẩm định → polish
4. **Chapter Assembly** — Ghép beat, đọc lại toàn chương, kiểm tra flow
5. **Continuity Scan** — Scan mỗi chương + mỗi arc
6. **Export EPUB** — Format, mục lục, metadata

## 10 Lỗi Chết Người

Xem chi tiết tại [references/loi-chet-nguoi.md](references/loi-chet-nguoi.md)

## Prompt Mẫu Sao Chép Ngay

Xem bộ prompt đầy đủ tại [references/prompt-mau.md](references/prompt-mau.md)

## Tương Thích

Hoạt động với mọi LLM: Claude, ChatGPT, Gemini, Grok, Mistral, LLaMA. Nạp system prompt qua Project Instructions, Custom Instructions, hoặc paste đầu cuộc hội thoại.
