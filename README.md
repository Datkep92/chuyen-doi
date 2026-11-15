# Chuyển PDF sang Word & Excel

Trang HTML chạy hoàn toàn trên trình duyệt (không server, không upload dữ liệu).

## Cách dùng

1. Mở `index.html` bằng trình duyệt (Safari/Chrome).
2. Kéo thả file PDF hoặc bấm **Chọn file PDF**.
3. Bấm **Phân tích PDF**.
4. Xem trước trang 1, sau đó bấm **Xuất Word (.docx)** hoặc **Xuất Excel (.xlsx)**.

## Yêu cầu

- Cần internet lần đầu để tải thư viện (pdf.js, SheetJS, docx.js, Tesseract.js) từ CDN; sau đó trình duyệt cache (offline).
- PDF scan ảnh: tự động OCR bằng Tesseract.js (vie+eng). Độ chính xác OCR phụ thuộc chất lượng ảnh.

## Ghi chú

- Excel: mỗi trang PDF → một sheet, giữ dạng bảng (hàng/cột).
- Word: nếu phát hiện bảng → tạo table; nếu không → đoạn văn.
- Số liệu được chuyển sang kiểu số trong Excel khi nhận dạng được.
- PDF scan ảnh: OCR có thể sai số/chữ; nên kiểm tra lại kết quả.
- PDF bố cục phức tạp (nhiều cột văn bản) có thể cần chỉnh tay.
