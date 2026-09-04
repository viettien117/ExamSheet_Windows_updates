# ExamSheet

**Phần mềm tạo phiếu trả lời trắc nghiệm** — cấu hình lần lượt từng phần của phiếu
(khung thông tin thí sinh, khung bong bóng mã số sinh viên, mã đề thi, phần trả lời
trắc nghiệm), ghép thành phiếu hoàn chỉnh rồi in hoặc xuất ra PNG / PDF / Word.
Phiếu in ra chấm được bằng [ExamScan](https://github.com/viettien117/ExamScan_Windows_updates).

Repo này host **bản cài đặt Windows mới nhất** và **kênh cập nhật tự động** cho ExamSheet.

> Bản macOS nằm ở repo riêng: [ExamSheet_macOS_updates](https://github.com/viettien117/ExamSheet_macOS_updates).

---

## Tải xuống bản mới nhất

1. Vào trang [**Releases**](https://github.com/viettien117/ExamSheet_Windows_updates/releases/latest)
2. Trong mục **Assets**, tải file `ExamSheet-x.y.z-x64.msi`
3. Bấm đúp file `.msi` → đi qua wizard cài đặt
4. Mở phần mềm từ **Start Menu** hoặc shortcut **Desktop** → "ExamSheet"

> Nếu Windows SmartScreen cảnh báo *"Windows protected your PC"*, bấm **More info** →
> **Run anyway** (file được ký bằng EdDSA của nhà phát triển).

## Yêu cầu hệ thống

- Windows 10 (64-bit) hoặc Windows 11
- Không cần cài .NET: bản cài đã kèm sẵn mọi thứ cần chạy

## Cập nhật tự động

Chương trình tự kiểm tra bản mới khi khởi động và mỗi 24 giờ, đọc file `appcast.xml`
trong chính repo này qua GitHub Pages. Bạn cũng có thể tự kiểm tra bất cứ lúc nào ở
trang **Cập nhật** trong chương trình.

## Ghi chú cho người bảo trì

File `.gitattributes` có từ commit đầu tiên và **không được xoá**: nó ghim
`appcast*.xml` ở chế độ nhị phân. Thiếu nó thì git tự đổi ký tự xuống dòng, chữ ký
Ed25519 lệch, và mọi máy đã cài vĩnh viễn không thấy bản cập nhật — **không một
thông báo lỗi nào chỉ ra nguyên nhân**.

Cũng **không được đổi tên hay di chuyển repo này**: địa chỉ appcast được biên dịch
thẳng vào từng bản phát hành. GitHub có chuyển hướng địa chỉ `github.com` sau khi đổi
tên, nhưng đường dẫn **GitHub Pages** thì không đảm bảo.

## Bản quyền

Copyright © 2026 RuBi. All rights reserved.
