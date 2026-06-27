# Catalog kiểu dáng pallet gỗ trên icdvietnam.com.vn → engine vẽ

Quét 2026-06-27 từ `/product-category/pallet-go/` (3 trang). Mọi kiểu dáng quy về **3 engine cấu trúc**, tham số hoá để vẽ được mọi sản phẩm.

## Engine
- **block** — chân cục: nan mặt + nan liên kết + lưới chân cục (NxM) + nan đáy. 1 hoặc 2 mặt.
- **stringer** — chân suốt: nan mặt + chân suốt chạy dọc chiều dài. Tuỳ chọn **khoét chân** (cắt 2 hốc/chân → 4 chiều nâng).
- **collar** — khung gỗ: 4 thành ván quây quanh chu vi, cao tuỳ chỉnh (biến pallet thành thùng).

## Ánh xạ sản phẩm → engine

| Sản phẩm trên site | Engine | Ghi chú cấu trúc |
|---|---|---|
| Pallet gỗ keo / thông / tràm / cao su / ép | block | Khác nhau ở chất liệu, cùng cấu trúc chân cục 2 mặt |
| Pallet gỗ 2 mặt 2 chiều nâng | block (2 mặt) | Tải 1000-1500kg, kê rack, chồng tầng |
| Pallet 1 mặt 4 chiều nâng thông thường / khoá chân | block (1 mặt) | 9 chân cục → 4 chiều nâng |
| Pallet gỗ tiêu chuẩn EPAL EU 800x1200x144 | block (1 mặt, vát nan dẫn) | 9 chân cục, 3 nan đáy chu vi, tải động 1500/tĩnh 4000 |
| EPAL 2 EU 1200x1000x162 | block | Họ EPAL, đổi kích thước |
| EPAL 3 EU 1000x1200x144 | block | Họ EPAL |
| EPAL 6 EU 800x600x144 (half) | block | Pallet nửa, ít chân hơn |
| EPAL CP1 1000x1200x138 | block | Pallet hoá chất, đáy chu vi |
| EPAL CP2 1140x1140 / 800x1200 (x138) | block | Mặt sàn gần kín |
| EPAL CP3 1140x1140x138 | block | |
| EPAL CP4 1100x1300x138 | block | |
| Loscam châu Á 1000x1200x156 | block | Đáy chu vi |
| Loscam kiểu Trung Quốc 1200x1000x156 | block | |
| Pallet gỗ 1 mặt 2 chiều nâng | stringer (không khoét) | 3 chân suốt, tải động 500/tĩnh 1000 |
| Pallet 1 mặt 4 chiều nâng khoét chân | stringer (khoét chân) | 3 chân suốt, mỗi chân khoét 2 hốc → 4 chiều, tải 200-300kg |
| Khung gỗ pallet 1200x800x195 | collar | Ván thông dày 20mm, bản lề thép, cao 195 |

Kích thước phần lớn "theo yêu cầu" → tool để người dùng nhập.

## Cách bố trí dropdown trong tool (2026-06-27)
Tool KHÔNG liệt kê từng sản phẩm (keo/thông/tràm... = cùng cấu trúc). Thay vào đó 2 dropdown:
- **Kiểu dáng** (cấu trúc): 5 lựa chọn = 2 mặt 2 chiều (chân suốt kín 2 bên + giữa, có sàn đáy) / 1 mặt 4 chiều khóa chân (chân cục) / 1 mặt 2 chiều chân suốt / 1 mặt 4 chiều khoét chân / khung gỗ.
  - LƯU Ý: "2 mặt 2 chiều" dùng engine CHÂN SUỐT (stringer) faces=2, KHÔNG dùng chân cục - vì chân kín suốt chiều dài nên chỉ nâng 2 đầu (2 chiều). Chỉ loại "khóa chân" (chân cục rời) mới 4 chiều.
- **Khổ / tiêu chuẩn** (chỉ đổi kích thước): 1100, 1200x1000, EPAL EU/2/3/6, CP1/CP2/CP4, Loscam Á/TQ.
- **Chất liệu** là ô nhập riêng (keo/thông/tràm/cao su/ép).

→ EPAL/CP/Loscam là KHỔ của kiểu "chân cục 1 mặt", không phải kiểu dáng riêng.
