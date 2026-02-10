# Mining (Khai thác từ vựng)

## Cài đặt Anki

Anki là phần mềm học tập bằng thẻ flashcard mạnh mẽ, hỗ trợ ghi nhớ dài hạn thông qua thuật toán lặp lại ngắt quãng. Phần mềm này hỗ trợ đa nền tảng, giúp bạn học mọi lúc mọi nơi.

### Windows/macOS/Linux

Để cài đặt trên máy tính, bạn truy cập trang chủ **[apps.ankiweb.net](https://apps.ankiweb.net/)**, tải phiên bản phù hợp với hệ điều hành đang dùng. Sau đó, chỉ cần chạy file cài đặt và thực hiện các bước xác nhận cơ bản (nhấn Next hoặc Enter) để hoàn tất.

### Android

Người dùng Android có thể tìm và tải **AnkiDroid** hoàn toàn miễn phí từ Google Play Store.

### iOS (iPhone/iPad)

Riêng với hệ điều hành iOS, bạn cần lưu ý đây là phiên bản trả phí. Bạn có thể tìm mua **AnkiMobile Flashcards** trên App Store với giá khoảng $24.99 (thanh toán một lần duy nhất).

## Cài đặt & cấu hình Yomitan

Yomitan là "trợ thủ" đắc lực giúp bạn tra cứu tiếng Nhật và tự động hóa việc tạo thẻ Anki. Để thiết lập quy trình này, bạn cần thực hiện theo các bước sau:

### Bước 1: Cài đặt tiện ích

Tùy vào trình duyệt bạn đang sử dụng, hãy thêm Yomitan từ cửa hàng tiện ích tương ứng:

- **Chrome/Edge**: Tìm kiếm trên Chrome Web Store.
- **Firefox**: Tìm kiếm trên Firefox Add-ons.

Đọc trên: [Wiki của Yomitan](https://yomitan.wiki/)

### Bước 2: Cài đặt Plugin AnkiConnect

Để Anki và Yomitan có thể "nói chuyện" được với nhau, bạn cần cài đặt AnkiConnect. Trong giao diện Anki, vào mục **Tools (Công cụ)** > **Add-ons (Tiện ích mở rộng)** > **Get Add-ons (Nhận tiện ích mở rộng)**. Sau đó, nhập mã số **`2055492159`** để hệ thống tự động cài đặt.

### Bước 3: Thêm dữ liệu từ điển

Yomitan cần dữ liệu để tra cứu. Bạn nhấp vào biểu tượng Yomitan trên trình duyệt, vào **Settings** > **Dictionaries**. Tại đây, hãy chọn **"Get recommended dictionaries…"** để cài các bộ từ điển được gợi ý từ chính Yomitan (Bạn cần phải chọn ngôn ngữ cho phù hợp).

### Bước 4: Cấu hình tích hợp Anki

Cuối cùng, trong phần **Settings** của Yomitan, bạn hãy gạt nút bật **"Enable Anki integration"**. Sau đó, chọn đúng bộ thẻ (deck) và kiểu ghi chú (note type) mà bạn muốn dùng để lưu trữ các từ vựng mới.

## "Mining" Với Yomitan

"Mining" là quá trình tạo thẻ học trực tiếp từ những nội dung tiếng Nhật thực tế mà bạn tiếp xúc hàng ngày.

### Chọn Note Type (Kiểu ghi chú)

Cấu trúc của thẻ Anki phụ thuộc vào Note Type.

### Ánh xạ trường dữ liệu (Anki card format)

Để thông tin từ Yomitan đổ vào đúng vị trí trên thẻ Anki, bạn cần cấu hình trong mục **Anki > Configure Anki card format...**. Dưới đây là cách ánh xạ các trường phổ biến:

| Trường trong Note Type | Cần điền gì vào |
| :--- | :--- |
| Từ vựng (Word) | `{expression}` |
| Định nghĩa (Meaning) | `{glossary}` hoặc `{glossary-brief}` |
| Câu ví dụ (Sentence) | `{cloze-prefix}<b>{cloze-body}</b>{cloze-suffix}` |
| Âm thanh (Audio) | `{audio}` |
| Ảnh minh họa (Picture) | *(Tự tìm rồi thêm sau, tìm trên <https://images.google.com/> chẳng hạn)* | 

#### Công cụ hỗ trợ Mining theo loại nội dung

Tùy vào nguồn tài liệu bạn đang xem mà chúng ta sẽ cần các công cụ "cầu nối" khác nhau để Yomitan có thể đọc được văn bản:

- **Đối với video trên Youtube hoặc phim trên Netflix chẳng hạn**: Sử dụng **asbplayer** để hiển thị phụ đề dạng văn bản có thể chọn được. Công cụ này còn giúp bạn tự động chụp ảnh và cắt đoạn âm thanh từ video vào thẻ Anki.
- **Đối với Visual Novels hoặc Game**: Sử dụng **Textractor** để trích xuất lời thoại từ game ra trình duyệt.
- **Đối với Sách điện tử (PDF, EPUB)**: Sử dụng **Ttsu Reader** hoặc **Yomitan PDF Reader** để có trải nghiệm đọc và tra cứu mượt mà nhất.
