# Some_terminal_commands - một số lệnh comment terminal
1. xem các danh sách các extension đã cài trong máy:
```
code --list-extensions
```
2. xuất danh sách các extension đã cài trong máy
```
code --list-extensions > extensions-list.txt
```
3. kiểm tra version của git
```
git --version 
```
4. kiểm tra phiên bản python
```
python --version
```
5. kiểm tra phiên bản của pip
```
pip --version
```
6. tạo môi trường ảo
```
python -m venv .venv
```
7. Chạy môi trường ảo
```
.\venv\Scripts\activate
```
8. Hủy kích hoạt môi trường ảo
```
deactivate
```
9. Cài đặt gói thư viện
```
pip install <name_package>
```
10. ghi danh sách các package thư viện đã cài vào requirements.txt
```
pip freeze > requirements.txt
```
11. cài các thư viện từ requirements.txt
```
pip install -r requirements.txt
```
12. Tạo gitignore
đến thư mục chứa dự án
```
echo.> .gitignore
```
13. đổi khoảng cách indent (khoảng thụt dòng)
ctrl + shift + p => Change tab display size => chọn 4 (mặc định)
15. cách tạo venv
tạo venv ngang cấp với folder chạy chương trình
vd:
- khachsan
+ .idea
+ app
+ venv

active như bình thường
```
.\venv\Scripts\activate
```
khi chạy file:
```
python -m app.index
```
```
python -m app.models
```
17. nếu tạo venv ở ngoài:
phải set PYTHONPATH
```
$env: PYTHONPATH = "D:\QLkhachSan\khachsan"
```
```
.venv\Scripts\python.exe khachsan\app\index.py
```
nếu không được thử set PYTHONPATH bằng cách này
```
set PYTHONPATH = D:\QLkhachSan\khachsan
```
```
.venv\Scripts\python.exe khachsan\app\index.py
```
21. 
    
