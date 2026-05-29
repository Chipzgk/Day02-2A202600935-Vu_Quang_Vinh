# Phase 7 — Individual Reflection (15')

## Tôi đã tham gia vào phần nào?

| Hoạt động | Đóng góp của tôi | Kết quả / Ảnh hưởng |
|---|---|---|
| **Scan & Pitch** | Đề xuất 10 vấn đề từ trải nghiệm bootcamp và cá nhân. Chọn pitch 3 bài toán thiết thực nhất. | Cung cấp đủ input cho nhóm, tạo ra 2 cụm chủ đề giúp mở rộng góc nhìn tiếp cận. |
| **Challenge** | Đánh giá chéo các ý tưởng dựa trên actor, workflow, bottleneck, impact và tính khả thi. | Giúp nhóm chốt được bộ tiêu chí chuẩn để lọc danh sách (shortlist). |
| **Workflow** | Đặt câu hỏi bóc tách quy trình CSKH với Dũng để hệ thống hóa luồng Before/After. | Xác định đúng điểm nghẽn ("nghe recording"), vẽ luồng mới giúp giảm thời gian QA từ 55' xuống 18'/call. |
| **Research** | Tìm hiểu cách thị trường giải quyết bài toán Auto-QA. | Định hướng nhóm đi theo mô hình Workflow thực tế thay vì làm Agent. |
| **Rule/Agent** | Phản biện ranh giới (Boundary), bảo vệ quan điểm AI chỉ "chuẩn bị thông tin". | Chốt AI làm tiền kỳ, con người (QA) duyệt cuối để đảm bảo an toàn. |

---

## Bảng dùng AI trong reflection

| Phase | Mục đích dùng AI | Điểm hữu ích | Điểm hời hợt / Sai sót | Cách tôi điều chỉnh |
|---|---|---|---|---|
| **Scan** | Brainstorm vấn đề bootcamp và sản xuất âm nhạc. | Cấu trúc ý mạch lạc, đa dạng góc nhìn. | Phân tích quy trình sản xuất âm nhạc chưa sát thực tế. | Lọc bỏ AI, giữ lại pain-point thật từ kinh nghiệm cá nhân trên các công cụ như Reaper hay BandLab. |
| **Research** | Tóm tắt tài liệu Auto QA thị trường & tìm case study. | Hiểu nhanh thuật ngữ CSKH; tìm ra pattern Scorecard phổ biến. | Gợi ý phân tích cảm xúc (sentiment) phức tạp; trích dẫn thiếu nguồn. | Gạt bỏ Sentiment, chỉ giữ tiêu chí Rule cứng và các case có link/số liệu verify được. |
| **Workflow** | Chuyển luồng QA thành sơ đồ ASCII. | Vẽ flow Before/After cực nhanh, dễ hình dung. | Lập lờ ranh giới trách nhiệm giữa AI và Người thật. | Chủ động thêm nhãn phân định rõ bước của AI và bước của QA. |
| **Problem** | Nhờ AI đóng vai "khách hàng" để bắt lỗi giải pháp. | Cảnh báo đúng rủi ro lộ dữ liệu (PII) từ file ghi âm. | Đề xuất mua tool bảo mật quá cồng kềnh, tốn kém. | Thêm rào cản thực tế vào bài: "Chỉ pilot bằng transcript đã ẩn danh". |

Reflection:

```text
Nhìn lại quá trình làm việc, tôi nhận ra các candidate mình đưa ra đều chỉ lấy bối cảnh chung của bootcamp. Đó là những vấn đề trong vùng an toàn, dễ hiểu và ai cũng thấy. Bởi vì tôi đã lo ngại việc mang những bài toán ngách, những nhức nhối thực sự trong chuyên môn hay công việc riêng của mình ra bàn luận vì sợ khó giải thích context cho nhóm hiểu, hoặc sợ nhóm không có sự đồng cảm.

Dũng đã làm được điều mà tôi không dám là mang một bài toán đặc thù vào nhóm. Dù ban đầu chúng tôi tốn thời gian để giải thích thuật ngữ, nhưng chính sự cụ thể, có số liệu thực tế và tính thực chiến của nó đã thay đổi cái nhìn của tôi. Một problem tốt đến từ trải nghiệm thực sự sâu sắc, chứ không phải từ những quan sát chung chung.

Vấn đề lúc đầu của tôi quá an toàn, nó rất khó để định lượng thành các bước giải quyết rành mạch. Trong khi bài toán ngách của Dũng vì quá rõ ràng về quy trình nên có thể vẽ ra được rule, workflow và ranh giới cho AI khá dễ dàng.
```