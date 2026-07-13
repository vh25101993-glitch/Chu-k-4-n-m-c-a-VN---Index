# Chu kỳ 4 năm của thị trường chứng khoán Việt Nam

Gói website tĩnh đã sẵn sàng triển khai lên Vercel.

## Cách 1 — Triển khai bằng Vercel CLI

1. Giải nén gói ZIP.
2. Mở Terminal trong thư mục dự án.
3. Chạy:

```bash
npm install -g vercel
vercel
```

4. Khi cần đưa lên môi trường production:

```bash
vercel --prod
```

Khi Vercel hỏi cấu hình, giữ nguyên thư mục hiện tại; dự án không cần Build Command hoặc Output Directory.

## Cách 2 — Triển khai qua GitHub

1. Tạo repository GitHub mới.
2. Đưa toàn bộ các file trong thư mục này lên repository.
3. Trên Vercel, chọn **Add New → Project** và import repository.
4. Framework Preset: **Other**.
5. Build Command và Output Directory: để trống.
6. Chọn **Deploy**.

## Cấu trúc gói

- `index.html`: báo cáo tài chính tương tác.
- `vercel.json`: URL sạch và security headers.
- `favicon.svg`: biểu tượng website.
- `site.webmanifest`: metadata cho trình duyệt và thiết bị di động.
- `robots.txt`: cấu hình thu thập dữ liệu.

## Lưu ý kỹ thuật

- Biểu đồ ECharts được tải qua CDN; thiết bị cần kết nối Internet để hiển thị biểu đồ.
- Báo cáo là website tĩnh, không cần Node.js runtime trên Vercel.
- Có thể đổi domain trong Vercel tại **Project Settings → Domains**.
