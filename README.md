# Sky-ASL Resource Pack

Pack đang dùng trên server Sky-ASL, bản `packreload1-20261008` (08/10/2026).
`general.zip` có nội dung giống hệt `pack.zip` đang phục vụ trên skyasl.xyz.

## Tải về và lưu bản sao

- [Bản mới nhất từ GitHub](https://raw.githubusercontent.com/TuanDanny/Sky-ASL-ResourcePack/main/general.zip)
- [Bản cố định ngày 08/10/2026](https://raw.githubusercontent.com/TuanDanny/Sky-ASL-ResourcePack/packreload1-20261008/general.zip)
- [Pack trên website](https://skyasl.xyz/pack.zip)
- [Bộ cài server đầy đủ](https://skyasl.xyz/SkyASL-TierVisuals-1.0.1-packreload1.zip)

Tag `packreload1-20261008` giữ bản này cố định khi `main/general.zip` có bản mới.
Các pack cũ vẫn nằm trong lịch sử Git. Bản trước: commit `0753c87d2a0876cb99453d630420bfeef6dbb5ba`.

```bash
curl -fL https://raw.githubusercontent.com/TuanDanny/Sky-ASL-ResourcePack/packreload1-20261008/general.zip -o general.zip
sha256sum general.zip
```

SHA256 cần khớp:
`0d5d030656e4de87140e2622066798a25edb4b13081f84d0a87181ec7443d3d5`.

SHA1: `a2b25655b79368082b409e32ba999c59c94ed007`; dung lượng 14.972.385 byte.
Chi tiết checksum và kết quả kiểm nằm trong [pack-info.json](pack-info.json).

## Nội dung và tương thích

Gom 800 bitmap provider thành 73 nhóm mỗi font, giữ nguyên 800 glyph, pixel và thông số chữ.
Minecraft 1.21.11 dùng một overlay thay cho tám; các định dạng khác giữ tài nguyên và thứ tự lớp cũ.
Không cắt model, texture, shader, GUI hay viền/tooltip tier. Gate kiểm 4.190 model, 898 texture,
3.090 định nghĩa tier và 8 bộ viền/tooltip đạt, không thiếu model/texture.

Trên client 1.21.11 đã thử, dựng lại tài nguyên sau khi tải mất 7,617 giây trong một lượt hợp lệ;
người chơi xác nhận hình ảnh đúng. Chưa thử trực tiếp client cũ hoặc đo ổn định trên mọi máy.

Source, config và công cụ build/cài server nằm ở [Sky_ASL](https://github.com/TuanDanny/Sky_ASL),
thư mục `tools/tier-visuals` và `scripts`. Luôn dùng builder cùng catalog/bộ cài đã kiểm;
không thay pack công bố bằng ZIP raw từ ItemsAdder/ResourcePackManager.
