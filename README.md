# HQTCSDL_DTAP_BT3
Thông tin sinh viên:
- Họ và tên: Trương Văn Hải
- MSSV: K235480106021
- Lớp: K59.KMT.K01

# Bài tập 3: Quản Lý Cầm Đồ
Tạo database: QuanLyCamDo
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/cdde9661-58e3-4ec0-9540-bef0a439c1d6" />

-- 1. Tạo Database 
CREATE DATABASE QuanLyCamDo
GO
USE QuanLyCamDo
GO


Tạo bảng khách hàng
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b22212ab-6b04-4114-945d-2bc2722a7ea9" />

Tạo bảng hợp đồng
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/83a519ef-fa77-44d5-85c2-3f4e5f1410af" />


Tạo bảng tài sản
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c7b31369-bd1a-413e-b085-bd19e0b9befa" />


Tạo bảng Lịch sử giao dịch (Audit Log)
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0742649d-3078-44c9-b04f-d7488bf6cc7d" />



Kiểm tra khách hàng đã tồn tại chưa, nếu chưa thì thêm mới
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9aa378f3-8237-47a0-b3f6-c16a93b5be20" />


Tính tiền hợp đồng
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d74f080e-3d47-4e15-82d4-88c2f01ad033" />

Kiểm tra lại
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1d6af553-0bb9-441c-8da5-0e48475b805e" />

ev3: Xử lý trả nợ và hoàn trả tài sản

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/2c5b19d4-1709-4c3a-896c-b9ec79306963" />

Test sp

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/cb28dce1-bf35-4503-99e2-52cc6c6a602e" />

ev4:Truy vấn danh sách nợ xấu (Nợ khó đòi)

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/6ad601b2-2c49-4876-88d8-23d119d27665" />
Kiểm Tra Lại
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/4811525c-96c6-40ff-9008-970f1a26c1a8" />
ev5:


- Viết một Trigger tự động chuyển trạng thái hợp đồng sang "Quá hạn (nợ xấu)" sau khi hợp đồng đang ở trạng thái "Đang vay" mà ngày vượt quá Deadline 1

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/df0cdec9-1de6-46f3-adfe-4a269837f260" />


- Viết một Trigger tự động chuyển trạng thái tài sản sang "Sẵn sàng thanh lý" sau khi hợp đồng đang ở trạng thái "Quá hạn (nợ xấu)" mà ngày vượt quá Deadline 2.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/dd6d3080-9153-4bc8-88aa-a93098adfbcf" />


- Viết một Trigger tự động chuyển trạng thái tài sản thành “Đã bán thanh lý” sau khi trạng thái của hợp đồng chuyển sang "Đã thanh lý".

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/62832e73-f527-4d3f-923f-1193dd5cd7eb" />


- Sự kiện Gia hạn hợp đồng: Khách đến trả toàn bộ tiền lãi tính đến thời điểm hiện tại để dời Deadline 1 và Deadline 2 sang một kỳ hạn mới để tránh bị tính lãi kép.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/72a45055-9bbd-4347-be10-df1585de5364" />

- Lịch sử hợp đồng (Audit Log): CSDL phải có bảng Log để ghi lại mỗi lần khách trả một ít tiền (Ngày trả, số tiền trả, người thu tiền). Tránh việc chỉ ghi đè số tổng nợ khiến mất dấu vết dòng tiền.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e82eefc3-a3db-42d6-a3fa-cc72612d9fa7" />



