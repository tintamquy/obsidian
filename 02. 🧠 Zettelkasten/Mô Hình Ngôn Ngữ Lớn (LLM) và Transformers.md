---
tags: [ai, kienthucnen]
aliases: [LLM, Large Language Model, Transformer Architecture]
---
# Mô Hình Ngôn Ngữ Lớn (LLM) & Kiến trúc Transformer

## Large Language Model (LLM) là gì?
Là một hệ thống trí tuệ nhân tạo được đào tạo trên khối lượng lớn dữ liệu văn bản để có khả năng hiểu, tóm tắt, dịch thuật, dự đoán và tạo ra văn bản giống như con người. Bản chất toán học của LLM là dự đoán từ tiếp theo (Next-token prediction).

## Kiến trúc Transformer (2017)
Trước năm 2017, AI xử lý ngôn ngữ dùng RNN/LSTM (xử lý từ từ trái sang phải, chậm và hay quên ngữ cảnh xa). Năm 2017, Google ra mắt bài báo "Attention Is All You Need", giới thiệu kiến trúc Transformer với cơ chế **Self-Attention**.

- **Self-Attention:** Thay vì đọc từng từ, AI đọc toàn bộ câu cùng lúc và tính toán "trọng số kết nối" giữa các từ. Nhờ đó, nó biết từ "Ngân hàng" trong câu "Tôi ra ngân hàng rút tiền" khác với "Tôi ngồi trên bờ ngân hàng sông" (Bank of the river).
- Khả năng tính toán song song giúp Transformer đào tạo nhanh hơn trên GPU, từ đó dẫn đến sự bùng nổ của GPT (Generative Pre-trained Transformer).

## Các thành phần chính của RAG (Retrieval-Augmented Generation)
Để khắc phục tình trạng AI "bịa chuyện" (Hallucination) hoặc không biết dữ liệu mới, người ta dùng RAG.
1. **Vector Database:** Biến tài liệu của bạn (ví dụ Kinh Phật) thành các con số (Vector/Embedding).
2. **Retrieval (Truy xuất):** Khi bạn hỏi, hệ thống tìm các câu văn có Vector gần giống với câu hỏi nhất.
3. **Generation (Tạo văn bản):** Nhét các câu văn tìm được vào Prompt, ép LLM trả lời dựa trên tài liệu đó.

---
🔗 **Liên kết**: [[MOC Trí Tuệ Nhân Tạo]], [[Kỹ thuật Prompt Engineering Cơ Bản]]
