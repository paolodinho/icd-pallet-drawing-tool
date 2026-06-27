# Tool tạo bản vẽ pallet gỗ từ thông số

Biến mô tả bằng chữ (số nan, kích thước nan, chân cục, nan đáy, chiều cao) thành **bản vẽ kỹ thuật chính xác** + spec sheet brand ICD, xuất ảnh PNG gửi khách.

## Cách dùng
- Mở `index.html` bằng trình duyệt (double-click, không cần cài gì).
- Nhập thông số bên trái → bấm **Vẽ lại bản vẽ**.
- Bấm **Tải ảnh PNG gửi khách** để xuất ảnh.

## Vì sao chính xác hơn ChatGPT
Bản vẽ là **hình học tham số** (vẽ bằng JavaScript): nhập 5 nan → ra đúng 5 nan, 9 cục → đúng 9 cục, mỗi lần như nhau. Không bị "lúc 5 nan lúc 7 nan" như AI sinh ảnh.

## Phủ mọi kiểu dáng pallet gỗ trên site (3 engine + 21 preset)
Xem `catalog.md` để biết ánh xạ từng sản phẩm → engine.
- **block (chân cục)**: nan mặt + nan liên kết + lưới chân cục NxM + nan đáy. Phủ: keo/thông/tràm/cao su/ép, 2 mặt 2 chiều, 1 mặt 4 chiều khóa chân, toàn bộ EPAL/CP, Loscam. (Block luôn có nan đáy đỡ chân; 1 mặt = 3 thanh chu vi, 2 mặt = sàn đáy.)
- **stringer (đà liền)**: nan mặt + đà dọc suốt chiều dài. Tick "khoét chân" → 2 hốc/đà = 4 chiều nâng. Phủ: 1 mặt 2 chiều, 1 mặt 4 chiều khoét chân.
- **collar (khung gỗ)**: 4 thành ván quây chu vi, cao tuỳ chỉnh. Phủ: khung gỗ pallet.

Chiều cao tổng tự tính theo các lớp cấu thành.

## Hướng phát triển tiếp (3 việc anh Thăng để tính sau)
- Vát cạnh nan dẫn hướng EPAL (cosmetic), kiểu chân chi tiết hơn.
- Nhập từ link sản phẩm web → tự điền thông số.
- Bản vẽ 2D (top/side view) đầy đủ cote như ảnh khách gửi.
- Đóng thành tool nội bộ trên web ICD cho sales tự dùng.

*Tạo 2026-06-27.*
