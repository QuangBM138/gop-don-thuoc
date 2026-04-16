# 🩺 Công Cụ Gộp Đơn Thuốc 2 Liên (Prescription Merger)

Một công cụ web đơn giản, hiệu quả giúp nhân viên y tế chuyển đổi đơn thuốc (hoặc tài liệu PDF khổ A4) từ **1 bản đơn lẻ** thành **2 liên A5 trên cùng một tờ A4 ngang**. 

Đặc biệt, công cụ sử dụng công nghệ render hình ảnh chất lượng cao để **giữ nguyên 100% hình ảnh chữ ký số, con dấu (SmartCA)** mà không làm mất chi tiết như các cách gộp PDF thông thường.

![GitHub Pages](https://img.shields.io/badge/Deployment-GitHub%20Pages-blue?style=for-the-badge&logo=github)
![JavaScript](https://img.shields.io/badge/Language-JavaScript-yellow?style=for-the-badge&logo=javascript)

## ✨ Tính năng nổi bật

* **Nhân đôi đơn thuốc:** Tự động chia khổ A4 ngang thành 2 phần A5 đều nhau, mỗi phần chứa 1 bản sao của trang gốc.
* **Bảo toàn chữ ký số:** Sử dụng thư viện PDF.js để "chụp ảnh" trang gốc ở độ phân giải cao (300 DPI), đảm bảo con dấu đỏ và chữ ký số hiển thị rõ nét khi in ấn.
* **Hỗ trợ nhiều trang:** Tự động xử lý tất cả các trang trong file PDF đầu vào (Ví dụ: file gốc có 2 trang đơn khác nhau -> kết quả sẽ có 2 trang A4 ngang, mỗi trang chứa 2 liên tương ứng).
* **Chạy hoàn toàn trên trình duyệt:** Không tải dữ liệu lên server, đảm bảo tính bảo mật cho thông tin bệnh nhân.
* **Giao diện thân thiện:** Dễ sử dụng, hỗ trợ cả trên máy tính và điện thoại.

## 🚀 Cách sử dụng

1.  Truy cập vào trang web: `https://quangbm138.github.io/gop-don-thuoc/`
2.  Nhấn nút **Chọn tệp** để tải lên file PDF đơn thuốc xuất từ hệ thống HIS.
3.  Nhấn nút **Xử lý tất cả các trang**.
4.  Chờ trong giây lát để hệ thống render và ghép liên.
5.  File PDF kết quả sẽ tự động được tải về máy. Bạn chỉ cần mở lên và in.

> **Lưu ý khi in:** Để có kết quả tốt nhất, hãy chọn khổ giấy **A4** và hướng giấy **Ngang (Landscape)** trong cài đặt máy in.

## 🛠 Công nghệ sử dụng

Công cụ này được xây dựng dựa trên các thư viện mã nguồn mở mạnh mẽ:
* [PDF.js](https://mozilla.github.io/pdf.js/): Được dùng để render các trang PDF thành hình ảnh chất lượng cao nhằm giữ lại lớp chữ ký số bảo mật.
* [pdf-lib](https://pdf-lib.js.org/): Được dùng để tạo tài liệu PDF mới, nhúng hình ảnh và căn chỉnh bố cục 2 liên.
* **GitHub Actions:** Tự động hóa quá trình deploy lên GitHub Pages mỗi khi có thay đổi code.

## 📁 Cấu trúc thư mục

```text
gop-don-thuoc/
├── .github/workflows/    # Cấu hình tự động Deploy GitHub Pages
├── index.html            # Giao diện chính và logic xử lý (Single Page)
└── README.md             # Tài liệu hướng dẫn
```

## 📝 Đóng góp

Nếu bạn phát hiện lỗi hoặc muốn cải tiến thêm tính năng (ví dụ: gộp 4 liên, thêm lề cắt...), vui lòng tạo **Issue** hoặc gửi **Pull Request**. Mọi sự đóng góp đều được trân trọng!

## 📄 Giấy phép

Dự án này được phát hành dưới giấy phép MIT. Tự do sử dụng cho mục đích cá nhân và y tế.

---
**Phát triển bởi [Minh Quang](https://github.com/quangbm138)**
