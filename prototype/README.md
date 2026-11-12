# Prototype T3 — "ok đổi đi" mơ hồ → đổi nhầm

## 1. `index.html` (mock, mở trực tiếp bằng trình duyệt)
- Ca khó: **Màn 1** (AI hỏi lại một câu + giữ chỗ) → **Chọn** chuyến → **Xác nhận đổi** → **"Mình đổi nhầm chuyến"** → **Màn 2** (không tự hoàn tác được: giữ chỗ chuyến đúng + chuyển nhân viên, kèm thẻ "nhân viên thấy sẵn").
- Ô mô phỏng lỗi: **chuyến vừa hết chỗ lúc xác nhận**; **hãng từ chối giữ chỗ**. Nhánh phụ: **"Thôi, hoàn vé"**, **Chữ to**, nút **"Báo: AI hiểu sai chỗ nào?"**, ô **"Ca lạ"** (bộ định tuyến từ khoá, không phải AI thật).
- Không có lời gọi AI trong file này.

## 2. `ai-live.html` (AI thật)
- Chạy qua link Claude: https://claude.ai/artifact/LRKDtZgvK78L14Y18KBvYE (mở file trực tiếp thì không gọi được AI).
- AI đọc tin khách và **chọn tool**; mã hệ thống kiểm tra và áp mức tự chủ (đổi chuyến luôn cần khách bấm, hoàn vé cần ô tích, bồi thường bị chặn). Không có API key trong trang.
- Log lời gọi: nút **"Tải log JSON"** → lưu thành `ai-log.json` trong thư mục này, kèm ảnh chụp `anh-8-ai-that.png`.

## Ảnh
`anh-1` đến `anh-7`. Bảng số ↔ nguyên tắc HAX/PAIR ↔ mức tự chủ nằm ở `../spec.md` §5.
