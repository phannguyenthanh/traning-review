Hãy đóng vai một chuyên gia lập trình Frontend. Nhiệm vụ của bạn là viết mã nguồn cho một ứng dụng Web PWA (Progressive Web App) dạng Flashcard để luyện phỏng vấn tiếng Anh, bao gồm 1 file duy nhất (index.html chứa cả CSS và JS).

YÊU CẦU CÔNG NGHỆ:
- Chỉ sử dụng HTML, CSS và Javascript thuần (Vanilla JS), tuyệt đối không dùng framework (React, Vue, Tailwind, v.v.).
- Không sử dụng API bên ngoài (trừ Web Speech API mặc định của trình duyệt).
- Phải có các thẻ meta cần thiết để hỗ trợ tính năng "Add to Home Screen" trên iOS/Android (hiển thị toàn màn hình như một native app).

YÊU CẦU TÍNH NĂNG:
1. Giao diện (UI):
- Giao diện Dark mode, hiện đại, tối giản dành cho lập trình viên.
- Hiển thị một thẻ bài (Card) ở giữa màn hình. Mặc định chỉ hiện Câu hỏi.
- Có nút "Lật thẻ" (hoặc click trực tiếp vào thẻ) để hiển thị Câu trả lời.
- Có nút "Câu trước" và "Câu tiếp".

2. Dữ liệu:
- Khởi tạo một mảng JSON hardcode khoảng 3-5 câu hỏi phỏng vấn IT bằng tiếng Anh. Mỗi object gồm { q: "Câu hỏi", a: "Từ khóa trả lời" }.

3. Âm thanh (Web Speech API):
- Sử dụng `window.speechSynthesis` để tự động đọc câu hỏi (bằng tiếng Anh) khi thẻ bài xuất hiện.
- Khi người dùng lật thẻ, tự động đọc câu trả lời.
- dùng giọng của trình duyệt hoặc máy để có thể chạy offline được

4. Chế độ lái xe (Auto-play):
- Thêm một nút "Nghe tự động". đầu tiên randome câu chạy xong mới bắt đầu chạy
- Khi bấm nút này, ứng dụng sẽ chạy vòng lặp: Đọc câu hỏi -> Dừng 2 giây -> Hiện và đọc câu trả lời -> Dừng 3 giây -> Tự chuyển sang câu tiếp theo.
5. chế độ luyện tập
- đầu tiên là random các câu vào mỗi câu chỉ cần đọc câu hỏi. khi đọc xong người dùng muốn lật thì click vào thẻ để lật hiện câu trả lời hoặc có thêm button next để click sẽ next sang câu khác 

6 danh sách các câu hỏi thì nên tạo 1 file json riêng
7 code đáp dứng đẻ chạy được ngay trên github tức là ko cần build gì cả chỉ file tĩnh là chạy được

Hãy chỉ cung cấp mã nguồn (code), không cần giải thích dài dòng.
