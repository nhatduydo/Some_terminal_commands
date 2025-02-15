## một số lệnh comment terminal  
# MỤC LỤC
1. [xem các danh sách các extension đã cài trong máy](#xem-các-danh-sách-các-extension-đã-cài-trong-máy)
2. [xuất danh sách các extension đã cài trong máy](#xuất-danh-sách-các-extension-đã-cài-trong-máy)
3. [kiểm tra version của git](#kiểm-tra-version-của-git)
4. [kiểm tra phiên bản python](#kiểm-tra-phiên-bản-python)
5. [kiểm tra phiên bản của pip](#kiểm-tra-phiên-bản-của-pip)
6. [tạo môi trường ảo](#tạo-môi-trường-ảo)
7. [Chạy môi trường ảo](#chạy-môi-trường-ảo)
8. [Hủy kích hoạt môi trường ảo](#hủy-kích-hoạt-môi-trường-ảo)
9. [Cài đặt gói thư viện](#cài-đặt-gói-thư-viện)
10. [ghi danh sách các package thư viện đã cài vào requirements.txt](#ghi-danh-sách-các-package-thư-viện-đã-cài-vào-requirements.txt)
11. [cài các thư viện từ requirements](#cài-các-thư-viện-từ-requirements)
12. [Tạo gitignore](#tạo-gitignore)
13. [đổi khoảng cách indent (khoảng thụt dòng)](#đổi-khoảng-cách-indent-khoảng-thụt-dòng)
14. [cách tạo venv](#cách-tạo-venv)
15. [nếu tạo venv ở ngoài](#nếu-tạo-venv-ở-ngoài)
16. [kiểm tra phiên bản python](#kiểm-tra-phiên-bản-python)
17. [thu gọn code trong vscode](#thu-gọn-code-trong-vscode)
18. [mở rộng code trong vscode](#mở-rộng-code-trong-vscode)
19. [Lỗi "Import 'streamlit' could not be resolved"](#lỗi-import-streamlit-could-not-be-resolved)
20. [Chọn đúng Interpreter](#chọn-đúng-interpreter)  
21. [các extensions hỗ trợ format code python](#các-extensions-hỗ-trợ-format-code-python)
22. [SSH](#ssh)
    - [kiểm tra phiên bản](#kiểm-tra-phiên-bản)
    - [tạo cặp khóa public và private](#tạo-cặp-khóa-public-và-private)
    - [chứng thực ssh](#chứng-thực-ssh)
    - [xóa tài khoản đang chạy](#xóa-tài-khoản-đang-chạy)
23. [git stash - lưu những thay đổi tạm thời vào thùng chứa tạm](#git-stash---lưu-những-thay-đổi-tạm-thời-vào-thùng-chứa-tạm)
24. [đưa file về trạng thái cũ như ban đầu](#đưa-file-về-trạng-thái-cũ-như-ban-đầu)
25. [chuyển file từ vùng xanh staging area quay lại đỏ working copy](#chuyển-file-từ-vùng-xanh-staging-area-quay-lại-đỏ-working-copy)
26. [bỏ file khi đã lỡ push lên server](#bỏ-file-khi-đã-lỡ-push-lên-server)














## xem các danh sách các extension đã cài trong máy
```
code --list-extensions
```
## xuất danh sách các extension đã cài trong máy
```
code --list-extensions > extensions-list.txt
```
## kiểm tra version của git
```
git --version 
```
## kiểm tra phiên bản python
```
python --version
```
## kiểm tra phiên bản của pip
```
pip --version
```
## tạo môi trường ảo
```
python -m venv .venv
```
## Chạy môi trường ảo
```
.\venv\Scripts\activate
```
## Hủy kích hoạt môi trường ảo
```
deactivate
```
## Cài đặt gói thư viện
```
pip install <name_package>
```
## ghi danh sách các package thư viện đã cài vào requirements.txt
```
pip freeze > requirements.txt
```
## cài các thư viện từ requirements
```
pip install -r requirements.txt
```
## Tạo gitignore
đến thư mục chứa dự án
```
echo.> .gitignore
```
## đổi khoảng cách indent (khoảng thụt dòng)
ctrl + shift + p => Change tab display size => chọn 4 (mặc định)

## cách tạo venv
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

## nếu tạo venv ở ngoài
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
## kiểm tra phiên bản python
```
py -0
```
## thu gọn code trong vscode
ctrl + shift + [
## mở rộng code trong vscode
ctrl + shift + ]
## format code html
ctrl + shift + f
## Lỗi "Import 'streamlit' could not be resolved"
thường xảy ra khi VS Code không thể tìm thấy thư viện streamlit trong môi trường Python hiện tại. Dưới đây là một số bước bạn có thể thử để khắc phục vấn đề này:
## Chọn đúng Interpreter
Nhấn Ctrl+Shift+P để mở Command Palette.
Gõ Python: ```Select Interpreter``` và chọn đúng phiên bản Python mà bạn đã cài đặt streamlit.
streamlit run chatbot.py
## các extensions hỗ trợ format code python
- black formatter
- pep8
- yapf
## SSH
## kiểm tra phiên bản
```
ssh -V
```
## tạo cặp khóa public và private
```
ssh-keygen
```
enter lấy mặc định
vào thường dẫn sẽ thấy 2 cặp khóa được tạo ra 
```
C:\Users\nhatduy\.ssh
```
gồm 2 loại: id_ed123 và id_ed123.pub
+ id_ed123 => khóa private key
+ id_ed123.pub => đây là khóa public key, khi vô công ty, nếu sếp yêu cầu đưa khóa cho ổng => đưa khóa public

## chứng thực ssh
- vào setting => SSH and GPG keys => new SSH => ghi title và paste ssh vô => oke
- kể từ thòi điểm chứng thực ssh => khi push lên là không cần chứng thực nữa
## xóa tài khoản đang chạy 
tìm kiếm: Credential Manager => Windows Credentials: chọn tài khoản github => remove

## git stash - lưu những thay đổi tạm thời vào thùng chứa tạm
- lưu những thay đổi tạm thời vào thùng chứ tạm
  ```
  git stash
  ```
- xem danh dánh đã lưu
  ```
  git stash list
  ```
- áp dụng lại stash
- + apply hết
    ```
    git stash apply
    ```
  + apply 1 cái nào đó
    ```
    git stash list
    ```
    ```
    git stash apply {name}
    ```
    
## đưa file về trạng thái cũ như ban đầu
```
git checkout namefile
```
ví dụ: git checkout text.txt
chỉ có tác dụng ở vùng đỏ (trước git add) khi chuyển qua xanh (sau khi git add) thì không còn tác dụng
## chuyển file từ vùng xanh stagging area quay lại đỏ working copy
nếu file đã thực hiện git add mà muốn quay lại thì thực hiện 
```
git reset filename
```
còn nếu đã lỡ nằm trên thùng chứa cục bộ luôn thì chỉ có thể reset thùng chứa lại 
## bỏ file khi đã lỡ push lên server
khi đã lỡ thực hiện tất cả bước: 
git add => git commit => git push mà muốn gỡ file đã push trên server thực hiện
```
git rm filename
```
```
git commit -m ""
```
```
git push origin main
```
