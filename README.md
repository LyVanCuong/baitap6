# baitap6
btvn 6 của sv: K225480106100_Lý Văn Cường_HQTCSDL
Bài tập 6: Hệ quản trị CSDL
Chủ đề: Câu lệnh Select
Yêu cầu bài tập: 
Cho file sv_tnut.sql (1.6MB)
1. Hãy nêu các bước để import được dữ liệu trong sv_tnut.sql vào sql server của em
2. dữ liệu đầu vào là tên của sv; sđt; ngày, tháng, năm sinh của sinh viên (của sv đang làm bài tập này)
3. nhập sql để tìm xem có những sv nào trùng hoàn toàn ngày/tháng/năm với em?
4. nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em?
5. nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em?
6. nhập sql để tìm xem có những sv nào trùng tên với em?
7. nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.
8. nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.
9. BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH.
10. HÃY NHẬP SQL ĐỂ LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV (TRÌNH BÀY QUÁ TRÌNH SUY NGHĨ VÀ GIẢI NHỮNG VỨNG MẮC)

DEADLINE: 23H59:59 NGÀY 25/4/2025

-------------------------------------------------------------------------------------------------------------
1. Các bước để import dữ liệu từ file sv_tnut.sql vào sql server:
   - B1: Sau khi kết nối tới sql server, chọn file ---> open ---> file...:
  
     ![image](https://github.com/user-attachments/assets/b8a1aa33-bb44-4218-b04c-dcd90ec814cc)

   - B2: Chọn đường dẫn tải file về vào chọn đúng file sv_tnut.sql:
  
     ![image](https://github.com/user-attachments/assets/1f997b65-6da6-48c2-bd7b-dd4de924ad46)

   - B3: Tạo database với tên sv_tnut để trùng với câu lệnh use[sv_tnut] của thầy(lệnh sử dụng database):
  
     ![image](https://github.com/user-attachments/assets/c69a7d35-a2b6-4c23-9300-af1cc7ae102e)

   - B3: Bôi đen câu lệnh use[sv_tnut] và câu lệnh tạo bảng SV để tạo ra bảng trước rồi mới nhập dữ liệu được:
  
     ![image](https://github.com/user-attachments/assets/08f0b4c9-9f88-44e6-a720-022cea05120f)
     
  Kết quả chúng ta thấy được database đã có bảng dbo.SV:

![image](https://github.com/user-attachments/assets/ee750f21-1f64-4414-9a48-421ed50ddf35)


   - B4: Bôi đen( chọn) các dòng lệnh Insert ( toàn bộ code còn lại) rồi chạy để nạp dữ liệu vào cho bảng SV:

     ![image](https://github.com/user-attachments/assets/f67530ba-3e88-42c9-97e3-f29a4c8685b9)


2. Truy vấn ra thông tin của em ( Lý Văn Cường) với dữ liệu đầu vào là tên; sđt; ngày, tháng, năm sinh

   - New Query để code truy vấn
   - Dùng câu lệnh SELECT các trường tên, ngày sinh, số điện thoại từ bảng SV where các trường = dữ liệu phù hợp với thông tin của em:
  
     ![image](https://github.com/user-attachments/assets/ff24dc2a-375b-4de0-b30e-444f9091f1e6)


3. Truy vấn những sinh viên trùng hoàn toàn ngày tháng năm sinh với em:

- Dùng câu lệnh day, month, year để lấy ra được ngày, tháng, năm từ cột ns có kiểu Date để so sánh:

  ![image](https://github.com/user-attachments/assets/40286e22-e267-44f6-aa4b-7972a4ea8c8b)

4. 


   ![image](https://github.com/user-attachments/assets/b6fb4cb6-1b5c-4027-a9dd-c4248eecba1f)



