# Chuyển PDF sang Word & Excel

Trang HTML chạy hoàn toàn trên trình duyệt (không server, không upload dữ liệu).

## Cách dùng

1. Mở `index.html` bằng trình duyệt (Safari/Chrome).
2. Kéo thả file PDF hoặc bấm để chọn.
3. Bấm **Phân tích PDF**.
4. Xem trước trang 1, sau đó bấm **Xuất Word (.docx)** hoặc **Xuất Excel (.xlsx)**.

## Yêu cầu

- PDF phải có text (không phải scan ảnh).
- Cần internet lần đầu để tải thư viện (pdf.js, SheetJS, docx.js) từ CDN; sau đó trình duyệt cache.

## Ghi chú

- Excel: mỗi trang PDF → một sheet, giữ bố cục dạng bảng (hàng/cột).
- Word: nếu phát hiện bảng → tạo table; nếu không → đoạn văn.
- Số liệu được chuyển sang kiểu số trong Excel khi nhận dạng được.
- PDF scan ảnh hoặc bố cục phức tạp (nhiều cột văn bản) có thể cần chỉnh tay.
