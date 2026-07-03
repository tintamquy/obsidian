---
tags: [ai, kienthucnen, prompt]
aliases: [Prompting]
---
# Kỹ Thuật Prompt Engineering Cơ Bản

Để khai thác tối đa sức mạnh của AI, bạn không chỉ "hỏi", mà phải "lập trình" câu lệnh (Prompt).

## 1. Khung Prompt Chuẩn (Khung CREATE hoặc CLEAR)
Một prompt xịn phải có đủ các yếu tố sau:
- **Role (Vai trò):** "Hãy đóng vai một nhà sư uyên bác về Hán Tạng..."
- **Task (Nhiệm vụ):** "Nhiệm vụ của bạn là dịch đoạn kinh sau sang tiếng Việt hiện đại."
- **Context (Bối cảnh):** "Đoạn kinh này thuộc hệ phái Đại Thừa, nói về tánh Không."
- **Constraint (Ràng buộc):** "Không dùng từ ngữ quá hàn lâm. Không dài quá 500 chữ."
- **Format (Định dạng):** "Trình bày dưới dạng bảng: Cột 1 là Hán tự, Cột 2 là Hán Việt, Cột 3 là Dịch nghĩa."

## 2. Kỹ Thuật Few-Shot Prompting
AI học qua ví dụ rất nhanh. Thay vì chỉ ra lệnh (Zero-shot), hãy cho nó vài ví dụ.
*Ví dụ:*
Định dạng tôi muốn:
- 天 -> Thiên (Trời)
- 地 -> Địa (Đất)
Bây giờ hãy làm tương tự với: 人, 心, 佛.

## 3. Kỹ Thuật Chain of Thought (Chuỗi suy nghĩ)
Ép AI phải suy luận từng bước trước khi đưa ra kết quả. Rất hữu ích khi phân tích logic hoặc toán học.
*Cú pháp thần thánh:* "Hãy suy nghĩ từng bước một" (Let's think step by step).

---
🔗 **Liên kết**: [[MOC Trí Tuệ Nhân Tạo]]
