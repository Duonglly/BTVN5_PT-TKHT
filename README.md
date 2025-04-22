# BTVN5_PT-TKHT
# BÀI TẬP VỀ NHÀ 05, Môn Hệ quản trị csdl.

SUBJECT: Trigger on mssql

A. Trình bày lại đầu bài của đồ án PT&TKHT:
1. Mô tả bài toán của đồ án PT&TKHT, 
   đưa ra yêu cầu của bài toán đó:
   -Tên đề tài: Phân tích và thiết kế hệ thống quản lý khách sạn
   -Khái quát nội dung đề tài:
     Nhân viên Đăng nhập hệ thống, điền thông tin khách hàng và xác nhận đặt phòng, sau đó sau khi thanh toán thì hệ thống lưu lại thông tin khách hàng và cập nhật trạng thái phòng.
3. Cơ sở dữ liệu của Đồ án PT&TKHT :
   Có database với các bảng dữ liệu cần thiết (3nf),
   Các bảng này đã có PK, FK, CK cần thiết
   ![Ảnh chụp màn hình 2025-04-21 095600](https://github.com/user-attachments/assets/8853ef62-195c-422a-ae77-a24681fb8eb7)

 
B. Nội dung Bài tập 05:
1. Dựa trên cơ sở là csdl của Đồ án
2. Tìm cách bổ xung thêm 1 (hoặc vài) trường phi chuẩn
   (là trường tính toán đc, nhưng thêm vào thì ok hơn,
    ok hơn theo 1 logic nào đó, vd ok hơn về speed)
   => Nêu rõ logic này!
3. Viết trigger cho 1 bảng nào đó, 
   mà có sử dụng trường phi chuẩn này,
   nhằm đạt được 1 vài mục tiêu nào đó.
   => Nêu rõ các mục tiêu 
4. Nhập dữ liệu có kiểm soát, 
   nhằm để test sự hiệu quả của việc trigger auto run.
5. Kết luận về Trigger đã giúp gì cho đồ án của em.

HƯỚNG DẪN CÁCH LÀM:

Hướng dẫn làm phần A: 
 - Chỉ cần nêu ra y/c của đồ án.
 - Không cần chụp quá trình làm ra db, tables.
 - Chỉ cần đưa ra db gồm các bảng nào,
   mỗi bảng có các trường nào, kiểu dữ liệu nào,
   và pk, fk, ck của các bảng.

Hướng dẫn làm phần B:
1. Sv tạo repo mới trên github, cho phép truy cập public.
2. Tạo file Readme.md, đầu file để thông tin cá nhân sv.
3. Tiếp theo đưa phần A vào file Reame.md .
3. Các thao tác làm trên csdl bằng phần mềm ssms.
4. Chụp ảnh màn hình quá trình làm.
5. Paste ngay vào Readme.md, 
   rồi gõ mô tả ảnh này làm gì, nhập gì, hay đạt được điều gì...
6. Có thể thêm những nhận xét hoặc kết luận
   cho việc bản thân đã hiểu rõ thêm về 1 vấn đề gì đó.
7. Lặp lại các step 4 5 6 cho đến khi hoàn thành yêu cầu của phần B.
8. Xuất các file sql chứa cấu trúc và data, up lên cùng repo.
9. Link đến repo cần mở được trực tiếp nội dung, 
   Paste link này vào file excel online ghim trên nhóm.
   Thầy sẽ dùng tool để check các link này.

DEADLINE: 23H59:59 NGÀY 23/04/2025

p/s:
 - Sv được phép tham khảo mọi nguồn, nhưng phải tự làm lại.
 - Đọc thêm nội quy học tập để biết các chế tài.
 - Đã đến lúc khẳng định bản thân và toả sáng!
 - Chỗ nào vướng mắc cứ share lên nhóm để cùng tháo gỡ.
   # DEMO CÁC BƯỚC THỰC HIỆN

   ## Tạo db gồm 5 bảng như hình vẽ
   ![image](https://github.com/user-attachments/assets/94674bd0-3e46-42ad-8709-8840fbf184f8)
   ## ảnh này để thầy giáo xem được trong các trường có những thuộc tính gì
   ![image](https://github.com/user-attachments/assets/d9f06e68-fe86-4a18-afd9-216b07204ec8)
   ## Ảnh này để thầy giáo thấy rõ khóa chính, khóa ngoại và kiểu dữ liệu của 2 bảng khách hàng và phòng
   ![Ảnh chụp màn hình 2025-04-21 112131](https://github.com/user-attachments/assets/e42785ca-694a-4ce8-93bf-e55ed6f5b6d3)
   ## Ảnh này để thầy giáo thấy rõ khóa chính, khóa ngoại và kiểu dữ liệu của 2 bảng đặt phòng và hóa đơn
   ![image](https://githuTheo dõi thay đổi tổng tiền dịch vụ của từng Booking và ghi lại lịch sử thay đổi vào bảng log
   ![image](https://github.com/user-attachments/assets/d3a67669-288c-4260-bcfb-8e1af378099e)

   ## Giá trị trước và sau khi thay đổi đều được hiển thị trên bảng này
    ![image](https://github.com/user-attachments/assets/6fb93107-9b93-44a5-8099-2c7c6cf9f853)








