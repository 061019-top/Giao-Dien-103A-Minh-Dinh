# Tổng hợp Kiến thức CSS

## 1. Nhóm Tổng quan & Màu sắc
### Cách nhúng CSS (Lesson 2)
- Inline (viết trong thẻ HTML)
- Internal (viết trong thẻ style)
- **External** (file .css riêng) -> *Nên dùng*
    - Dễ quản lý code
    - Cache trình duyệt tốt hơn

### Hệ màu (Lesson 4)
- **HEX**: Phổ biến nhất (VD: #FF0000)
- **RGB/RGBA**: Quan trọng khi cần độ trong suốt
    - VD: rgba(0, 0, 0, 0.5) là đen mờ 50%

## 2. Nhóm Văn bản & Font
### Text Properties (Lesson 5)
- **text-align**: Căn lề (left, center, right, justify)
- **text-decoration**: Bỏ gạch chân link (none)
- **line-height**: Độ cao dòng (khoảng 1.5 - 1.6)

### Font Properties (Lesson 6)
- **font-family**: Quy định phông chữ
    - Luôn cần "fallback font" (font dự phòng)
    - VD: Arial, sans-serif

## 3. Nhóm Selectors (Lesson 7-10)
### ID vs Class (Lesson 8)
- **ID (#)**: Duy nhất (Header, Footer)
- **Class (.)**: Dùng nhiều lần (Button, Card)

### Combinators (Lesson 9)
- **Hậu duệ (Space)**: `div p` -> Chọn tất cả con cháu
- **Liền kề (+)**: `div + p` -> Chọn p ngay sau div

### Attribute Selector (Lesson 10)
- Chọn theo thuộc tính
- VD: `input[type="text"]` khác `input[type="submit"]`

## 4. Nhóm Nâng cao & Độ ưu tiên
### Pseudo-class & Element (Lesson 11)
- **:hover**: Khi di chuột vào
- **::before / ::after**: Phần tử giả trang trí

### Độ ưu tiên (Specificity) (Lesson 12)
- *Xếp hạng sức mạnh:*
    1. !important (Mạnh nhất - hạn chế dùng)
    2. Inline style
    3. ID Selector (#)
    4. Class Selector (.)
    5. Tag Selector (div, p) (Yếu nhất)