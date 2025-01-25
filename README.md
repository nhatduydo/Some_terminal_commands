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

14. cách tạo venv
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

15. nếu tạo venv ở ngoài:
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
16. kiểm tra phiên bản python
```
py -0
```
17. thu gọn code trong vscode (blue)
ctrl + shift + [
18. mở rộng code trong vscode (blue)
ctrl + shift + ]
19. format code html
ctrl + shift + f
20. Lỗi "Import 'streamlit' could not be resolved"
thường xảy ra khi VS Code không thể tìm thấy thư viện streamlit trong môi trường Python hiện tại. Dưới đây là một số bước bạn có thể thử để khắc phục vấn đề này:
Chọn đúng Interpreter:
Nhấn Ctrl+Shift+P để mở Command Palette.
Gõ Python: Select Interpreter và chọn đúng phiên bản Python mà bạn đã cài đặt streamlit.
streamlit run chatbot.py
