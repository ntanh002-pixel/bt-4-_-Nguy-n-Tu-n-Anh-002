# bt-4-_-Nguyen-Tuan-Anh-002
tạo cơ sở dữ liệu thời khoá biểu
 - Nguồn dữ liệu: TMS.tnut.edu.vn
 - Tạo các bảng tuỳ ý (3nf)
 - Tạo được query truy vấn ra thông tin gồm 4 cột: họ tên gv, môn dạy, giờ vào lớp, giờ ra.
   trả lời câu hỏi: trong khoảng thời gian từ datetime1 tới datetime2 thì có những gv nào đang bận giảng dạy.

các bước thực hiện:
1. Tạo github repo mới: đặt tên tuỳ ý (có liên quan đến bài tập này)
2. tạo file readme.md, edit online nó:
   paste những ảnh chụp màn hình
   gõ text mô tả cho ảnh đó

Gợi ý:
  sử dung tms => dữ liệu thô => tiền xử lý => dữ liệu như ý (3nf)
  tạo các bảng với struct phù hợp
  insert nhiều rows từ excel vào cửa sổ edit dữ liệu 1 table (quan sát thì sẽ làm đc)
  

deadline: 15/4/2025

- TẠO BẢNG GIẢNG VIÊN  
![Screenshot (216)](https://github.com/user-attachments/assets/d2518cd5-e141-4883-b420-47b91c2c6b23)

- TẠO BẢNG LỚP HỌC
![Screenshot (217)](https://github.com/user-attachments/assets/91a3c1a4-0ee7-4ab5-a1c6-735710b45e92)

- TẠO BẢNG MÔN HỌC
![Screenshot (218)](https://github.com/user-attachments/assets/ae80b7f7-aaae-4646-8812-1beafdd0535d)

- TẠO BẢNG PHÒNG HỌC
![Screenshot (220)](https://github.com/user-attachments/assets/2a4fcee8-4c5a-4a63-ad2a-0a3c84da0154)

- TẠO BẢNG THỜI KHOÁ BIỂU
![Screenshot (221)](https://github.com/user-attachments/assets/5615b084-c7a2-47bf-b46d-6c585cac07d1)

- TẠO SƠ ĐỒ:
  sau khi cài khoá chính và khoá ngoại thì được sơ đồ này :
![Screenshot (222)](https://github.com/user-attachments/assets/029c9c18-94f5-4fbf-b5fa-4199c15300a2)

- COPY từ Nguồn dữ liệu: TMS.tnut.edu.vn --> có các bảng sau:
- đây là dữ liệu của bảng GiangVien

![Screenshot (228)](https://github.com/user-attachments/assets/ce7d4264-cd2f-4422-89aa-28204153a5e0)

- đây là dữ liệu của bảng LopHoc:
  ![Screenshot (229)](https://github.com/user-attachments/assets/ddc55e26-7edf-4355-8762-358081e8856d)

- Đây là dữ liệu của bảng MonHoc:
![Screenshot (235)](https://github.com/user-attachments/assets/338a83fb-4a29-4fb2-af42-6a1d0b38b462)

- Đây là dữ liệu của bảng PhongHoc:
![image](https://github.com/user-attachments/assets/77102c30-afd8-4d8a-bb8b-d2e463b5148d)

- Đây là dữ liệu của bảng ThoiKhoaBieu:
  ![image](https://github.com/user-attachments/assets/913bef54-87ae-4980-8ae3-23fdc34aa56f)

-  Truy vấn ra thông tin gồm 4 cột: họ tên gv, môn dạy, giờ vào lớp, giờ ra:
  ![Screenshot (231)](https://github.com/user-attachments/assets/d1d08640-8515-4677-a2ca-2f4edd7e3efa)


- trả lời câu hỏi: trong khoảng thời gian từ datetime1 đến datetime2 có những giảng viên nào đang bận giảng dạy, điều kiện GioVao < datetime2 và GioRa > datetime1 đảm bảo có giao nhau trong khoảng thời gian đang xét, DISTINCT dùng để tránh trùng tên giảng viên nếu họ dạy nhiều lớp trong khoảng đó.

![Screenshot (232)](https://github.com/user-attachments/assets/c5fbd9be-65f1-4651-852f-9bfb1122e2f8)
