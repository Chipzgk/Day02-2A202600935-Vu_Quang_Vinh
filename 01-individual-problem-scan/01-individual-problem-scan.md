## 01 — Individual Problem Scan
## Scan rộng

| # | Lăng kính | Problem quan sát được | Ai đang đau? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Tốn thời gian | Khó nắm bắt được các thông tin do có quá nhiều kênh thông báo. | Học viên | Học viên hay đi nhầm phòng, lỡ deadline do trôi tin; hoặc mỗi tối phải tự lướt 4-5 app khác nhau chụp màn hình lại để không quên việc. |
| 2 | AI có thể làm tốt hơn | Học viên nhiều nhưng trợ giảng ít dẫn đến việc thắc mắc nhưng không được giải đáp. | Học viên | Tiến độ thực hành bị "đóng băng", học viên phải copy code của nhau hoặc tự mang lên StackOverflow/AI hỏi thay vì chờ TA. |
| 3 | AI có thể làm tốt hơn | Kiến thức nhiều và nặng, dẫn đến cần phải note để xem lại. | Học viên | TA phải copy-paste cùng một câu trả lời hướng dẫn địa điểm/quy trình tới 20 lần trong các đoạn chat cá nhân khác nhau mỗi ngày. |
| 4 | Lặp lại | Các học viên đều có những thắc mắc giống nhau. | Trợ giảng | Mất trắng 45 phút đầu của ca thực hành chiều chỉ để TA đi fix lỗi biến môi trường (environment variables) cho từng máy cá nhân thay vì tập trung hướng dẫn logic thuật toán. |
| 5 | AI có thể làm tốt hơn | Việc tra cứu khó khăn vì kiến thức quá nhiều và rải rác, slide quá dài và nặng tính thuật ngữ chuyên môn. | Học viên | Học viên copy các thuật ngữ trong slide ném ra ngoài web hoặc nhờ công cụ khác gen ra đoạn code ví dụ minh họa mới có thể hiểu được. |
| 6 | Cải thiện sản phẩm người dùng | App điểm danh hay bị lỗi vặt. | Học viên | Học viên liên tục phải chụp ảnh màn hình lỗi app gửi vào group chat lớp để làm minh chứng, hoặc giảng viên phải lấy giấy ra điểm danh miệng. |
| 7 | Lặp lại | Các khách hàng sau khi thu âm xong đều phải clean vocal. | Mixer | Mixer luôn luôn phải điều chỉnh/gọt dũa lại vocal cho khách gây tốn nhiều thời gian mix và master. |
| 8 | Cải thiện sản phẩm người dùng | Các khách hàng khi muốn điều chỉnh sau thu âm thường đưa ra những yêu cầu rất chung chung. | Mixer | Mixer luôn phải trao đổi lại với khách để có thể hiểu ý muốn thật sự của khách hàng. |
| 9 | Tốn thời gian | Khi muốn ghép vocal vào beat mới đều phải tự căn lại từng nhịp/pitching lại. | Mixer | Mất nguyên cả một buổi tối chỉ để ngồi căng mắt "nắn" từng chữ một cho hai giọng hát trùng khớp nhau, chưa kịp làm hiệu ứng gì hay ho thì tai đã mệt mỏi và tụt hết cảm hứng. |
| 10 | Tốn thời gian | Soạn nốt nhạc (chuỗi MIDI) thủ công cho hàng loạt nhạc cụ khác nhau dựa trên cùng một vòng hợp âm gốc. | Producer | Tự vẽ hàng trăm nốt nhạc rập khuôn trên màn hình. Mất trắng cả tiếng đồng hồ để "copy-paste - sửa nốt" nhàm chán để dựng khung bài, làm đứt gãy hoàn toàn luồng cảm xúc ban đầu. |

## Top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Học viên nhiều nhưng trợ giảng ít dẫn đến việc thắc mắc nhưng không được giải đáp. | Vì gây ra tình trạng hoảng loạn ở học viên. | Có phải mọi câu hỏi đều thực sự cần TA là người thật giải đáp? (Hay 80% trong số đó chỉ là lỗi cấu hình môi trường, syntax cơ bản mà một AI Agent có thể đọc log và tự động gỡ lỗi thay TA?) |
| 2 | Các học viên đều có thắc mắc giống nhau. | Gây ra tình trạng mệt mỏi ở giảng viên. | Tại sao học viên lại đi hỏi thay vì tự tra cứu? (Do trường chưa có bộ tài liệu FAQ chuẩn, do wiki quá khó tìm, hay đơn giản là do thói quen ỷ lại/lười đọc của học viên?) |
| 3 | Khó nắm bắt được các thông tin do có quá nhiều kênh thông báo. | Gây ra sự hoang mang và bối rối của học viên vì sợ lỡ thông báo. | Nếu xây dựng một công cụ gom mọi thông báo về một nơi, liệu học viên có dùng không? (Hay công cụ đó lại vô tình trở thành "kênh thông báo thứ N+1" khiến tình trạng nhiễu loạn nặng nề hơn?) |

## Problem Card #1

**Problem 1 câu:**  
Học viên bị "đóng băng" tiến độ thực hành vì không được giải đáp kịp thời do số lượng trợ giảng quá ít so với học viên.

**Actor:**  
Học viên

**Thời điểm / bối cảnh:**  
Trong các buổi thực hành lab, đặc biệt khi gặp lỗi cấu hình môi trường hoặc thắc mắc về syntax.  
Bùng phát đầu kỳ khi học viên mới setup môi trường lần đầu.

**Current workflow:**

```text
CURRENT STATE — Học viên có thắc mắc trong lab

+--------------------+     +--------------------+     +--------------------+
| 1 Học viên gặp     | --> | 2 Giơ tay hoặc     | --> | 3 Chờ TA đang     |
|   lỗi/thắc mắc    |     |   nhắn tin gọi TA  |     |   bận chỗ khác    |
|                    |     |                    |     |   🔴              |
+--------------------+     +--------------------+     +--------------------+
                                                               |
                                                               v
+--------------------+     +--------------------+     +--------------------+
| 6 Tiến độ đóng     | <-- | 5 Copy code bạn    | <-- | 4 Không chờ được  |
|   băng hoặc bỏ     |     |   hoặc hỏi         |     |   → tự xoay sở    |
|   dở lab           |     |   ChatGPT/SO       |     |                   |
+--------------------+     +--------------------+     +--------------------+

🔴 = Bottleneck: TA đang bận hướng dẫn người khác, không thể phân thân.
```

**Bottleneck:**  
Trợ giảng đang bận hướng dẫn người khác, không đủ nhân lực phục vụ đồng thời nhiều học viên.

**Impact:**  
Học viên hoảng loạn và bối rối do bị cuống.  
Tiến độ thực hành bị đình trệ.  
Học viên copy code thay vì tự hiểu, giảm chất lượng học.

**Success metric:**  
Thời gian chờ trung bình được giải đáp của học viên giảm xuống.

**Non-AI alternative:**  
Tăng số lượng trợ giảng.

**AI hypothesis:**  
Nếu chúng ta xây dựng một hệ thống Virtual TA Agent được nhúng trực tiếp vào nền tảng chat hoặc môi trường học tập, được cấp bộ nhớ chứa toàn bộ tài liệu giảng dạy và FAQ của môn học, Agent này có thể tự động đọc log lỗi hoặc thắc mắc của học viên, suy luận và đưa ra hướng dẫn từng bước ngay lập tức. Điều này sẽ lọc hết các sự cố lặp lại, chỉ đẩy những lỗi logic phức tạp lên cho TA con người.

**Quick gut:**  
Agent

### Draft future workflow

```text
FUTURE STATE — Học viên có thắc mắc trong lab (với Virtual TA)

+--------------------+     +--------------------+     +--------------------+
| 1 Học viên gặp     | --> | 2 Hỏi Virtual TA   | --> | 3 Agent đọc log   |
|   lỗi/thắc mắc    |     |   Agent            |     |   + tìm trong     |
|                    |     |                    |     |   tài liệu        |
+--------------------+     +--------------------+     +--------------------+
                                                               |
                                                               v
+--------------------+     +--------------------+     +--------------------+
| 6 TA con người     | <-- | 5 Câu hỏi khó/mới  | <-- | 4 Agent trả lời   |
|   xử lý ca khó    |     |   được tag TA thật |     |   từng bước ngay  |
|   10' 🟢           |     |                    |     |   lập tức         |
+--------------------+     +--------------------+     +--------------------+

🟢 = Human boundary: TA con người chỉ xử lý lỗi logic phức tạp hoặc câu hỏi ngoài tài liệu.
Fallback: Agent không chắc → tag TA thật và đính kèm context để TA xử lý nhanh hơn.
```

## Problem Card #2

**Problem 1 câu:**  
Trợ giảng bị quá tải và mệt mỏi do phải lặp đi lặp lại thao tác trả lời những thắc mắc giống hệt nhau từ nhiều học viên.

**Actor:**

* Trợ giảng (TA) / Giảng viên

**Thời điểm / bối cảnh:**

* Xảy ra liên tục trong suốt học kỳ
* Đặc biệt bùng phát vào đầu kỳ khi học viên bỡ ngỡ setup môi trường mới
* Hoặc ngay trước các kỳ thi/deadline bài tập lớn

**Current workflow:**

```text
CURRENT STATE — TA xử lý câu hỏi lặp lại từ nhiều học viên

+--------------------+     +--------------------+     +--------------------+
| 1 Học viên A, B, C | --> | 2 Từng người nhắn  | --> | 3 TA mở và đọc   |
|   cùng gặp một    |     |   tin riêng lẻ qua |     |   từng tin một    |
|   vấn đề          |     |   Zalo/Teams/Email |     |                   |
+--------------------+     +--------------------+     +--------------------+
                                                               |
                                                               v
+--------------------+     +--------------------+     +--------------------+
| 6 TA gõ/dán lại    | <-- | 5 TA tự nhớ lại    | <-- | 4 TA nhận ra đây  |
|   câu trả lời      |     |   hoặc lục tìm     |     |   là lỗi phổ biến |
|   thủ công từng    |     |   chat cũ để copy  |     |   đã từng gặp     |
|   người 🔴        |     |                    |     |                   |
+--------------------+     +--------------------+     +--------------------+

🔴 = Bottleneck: TA lãng phí thời gian copy-paste thủ công thay vì xử lý câu hỏi chuyên sâu.
```

**Bottleneck:**  
Bước 5 và 6: TA lãng phí thời gian quý giá chỉ để làm công việc copy-paste như một cái máy, thay vì dùng chuyên môn để hỗ trợ các ca khó.

**Impact:**  
Gây mệt mỏi, chán nản và hao mòn năng lượng cho TA.  
Làm giảm chất lượng hỗ trợ tổng thể vì TA không còn đủ thời gian và sức lực cho những câu hỏi đòi hỏi tư duy logic chuyên sâu.

**Success metric:**  
Giảm 80% số lượng tin nhắn hỏi các vấn đề lặp lại/cơ bản gửi trực tiếp đến TA.  
Tiết kiệm tối thiểu 2 giờ làm việc mỗi tuần cho mỗi trợ giảng.

**Non-AI alternative:**

* Soạn một tài liệu FAQ (Google Docs hoặc Notion) thật dài và ghim lên group lớp (thường thất bại vì học viên lười tự đọc).
* Sử dụng Rule-based Chatbot (cài sẵn kịch bản: gõ từ khóa "tòa A" thì trả lời địa chỉ).
* Đào tạo ban cán sự lớp để chia sẻ gánh nặng trả lời thay TA.

**AI hypothesis:**  
Nếu sử dụng một AI Agent đóng vai trò "tiền tuyến" (Frontline Support) được nhúng vào group chat, có quyền truy cập lịch sử chat và tài liệu môn học, nó có thể tự động phân tích ý định (intent) của câu hỏi. Nếu là câu hỏi trùng lặp, Agent sẽ tự động trả lời ngay lập tức, chỉ tag TA vào khi gặp câu hỏi mới hoặc câu hỏi khó.

**Quick gut:**  
Agent

### Draft future workflow

```text
FUTURE STATE — AI Agent xử lý câu hỏi lặp lại thay TA

+--------------------+     +--------------------+     +--------------------+
| 1 Học viên A, B, C | --> | 2 AI Agent nhận    | --> | 3 Agent phân tích |
|   gửi câu hỏi vào |     |   tin nhắn trong   |     |   intent + đối    |
|   group chat       |     |   group chat       |     |   chiếu tài liệu  |
+--------------------+     +--------------------+     +--------------------+
                                                               |
                                                               v
+--------------------+     +--------------------+     +--------------------+
| 6 TA chỉ xử lý     | <-- | 5 Câu hỏi mới/khó  | <-- | 4 Câu hỏi lặp →   |
|   câu khó,         |     |   → Agent tag TA   |     |   Agent tự trả    |
|   tiết kiệm 2h/    |     |   kèm context      |     |   lời ngay        |
|   tuần 🟢          |     |                    |     |                   |
+--------------------+     +--------------------+     +--------------------+

🟢 = Human boundary: TA chỉ được tag khi câu hỏi vượt quá tài liệu hiện có hoặc cần phán đoán chuyên môn.
Fallback: Agent không chắc intent → hỏi lại học viên để làm rõ trước khi trả lời hoặc tag TA.
```

## Problem Card #3

**Problem 1 câu:**  
Học viên hoang mang và dễ lỡ việc do phải tự thu thập và trích xuất thông tin, deadline từ quá nhiều kênh thông báo khác nhau.

**Actor:**

* Học viên

**Thời điểm / bối cảnh:**

* Hằng ngày, đặc biệt là vào buổi tối khi học viên cần sắp xếp lại công việc hoặc lên kế hoạch cho ngày hôm sau

**Current workflow:**

```text
CURRENT STATE — Học viên quản lý thông báo từ nhiều kênh

+--------------------+     +--------------------+     +--------------------+
| 1 Nhà trường/GV    | --> | 2 Học viên mở lần  | --> | 3 Đọc dò từng     |
|   gửi thông báo    |     |   lượt từng app    |     |   tin để chắt     |
|   trên Teams,      |     |   (Teams, Zalo,    |     |   lọc thông tin   |
|   Zalo, Email      |     |    Email)          |     |   trọng tâm 🔴    |
|                    |     |                    |     |                   |
+--------------------+     +--------------------+     +--------------------+
                                                               |
                                                               v
+--------------------+     +--------------------+     +--------------------+
| 6 Bới tìm lại khi  | <-- | 5 Quên ghi chú →   | <-- | 4 Chụp màn hình   |
|   cần đến          |     |   lỡ sự kiện/      |     |   hoặc tự gõ lại  |
|                    |     |   deadline         |     |   vào app nhắc    |
+--------------------+     +--------------------+     +--------------------+

🔴 = Bottleneck: phải "đi săn" thông báo ở nhiều nơi và trích xuất bằng mắt thường, tốn thời gian và dễ sai sót.
```

**Bottleneck:**  
Bước 2 và 3: Việc phải chủ động kiểm tra thông báo ở nhiều nơi và trích xuất thông tin quan trọng bằng mắt thường cực kỳ tốn thời gian và dễ sai sót.

**Impact:**  
Tạo ra trạng thái tâm lý FOMO (luôn sợ lỡ thông báo quan trọng) gây hoang mang, bối rối.  
Dẫn đến các hậu quả thực tế như đi nhầm phòng học, quên mang tài liệu, hoặc nộp bài muộn.

**Success metric:**  
Học viên chỉ mất dưới 2 phút mỗi tối để nắm được toàn bộ hành động cần làm cho ngày mai.  
Tỷ lệ lỡ sự kiện/deadline do trôi thông báo giảm xuống 0.

**Non-AI alternative:**

* Thống nhất quy định toàn trường chỉ dùng DUY NHẤT một kênh thông báo (về mặt hành chính là bất khả thi).
* Cử một ban cán sự lớp chuyên tổng hợp mọi tin nhắn và gửi 1 bản tin tóm tắt mỗi sáng.
* Dùng các tool Automation (Make/Zapier) gom tất cả tin nhắn về chung 1 luồng (nhưng học viên vẫn phải tự đọc khối lượng chữ khổng lồ đó).

**AI hypothesis:**  
Nếu chúng ta xây dựng một hệ thống Workflow tự động thu thập dữ liệu thô từ các nền tảng (via Webhooks/API) đẩy về một nguồn duy nhất, sau đó dùng AI (LLM) để đọc hiểu, bóc tách chính xác các "Action items" và tự động tạo ra file lịch sự kiện (.ics) hoặc push vào app To-do list cho học viên, thì học viên sẽ hoàn toàn được giải phóng khỏi việc quản lý thông báo.

**Quick gut:**  
Workflow

### Draft future workflow

```text
FUTURE STATE — Học viên nhận tóm tắt hành động tự động mỗi tối

+--------------------+     +--------------------+     +--------------------+
| 1 Thông báo từ     | --> | 2 Webhook/API tự   | --> | 3 AI (LLM) đọc    |
|   Teams, Zalo,     |     |   động gom về      |     |   hiểu và bóc     |
|   Email            |     |   một nguồn duy    |     |   tách Action     |
|                    |     |   nhất             |     |   items           |
+--------------------+     +--------------------+     +--------------------+
                                                               |
                                                               v
+--------------------+     +--------------------+     +--------------------+
| 6 Học viên chỉ     | <-- | 5 Push vào To-do   | <-- | 4 Tạo file .ics   |
|   cần 2 phút/tối  |     |   list hoặc gửi    |     |   hoặc bản tin    |
|   để nắm việc cần |     |   bản tin tóm tắt  |     |   tóm tắt         |
|   làm 🟢          |     |   cho học viên     |     |                   |
+--------------------+     +--------------------+     +--------------------+

🟢 = Human boundary: ban cán sự hoặc giảng viên kiểm tra và xác nhận bản tin tóm tắt trước khi gửi nếu cần.
Fallback: Webhook bị lỗi hoặc thiếu API → ban cán sự gửi bản tóm tắt thủ công như backup.
```