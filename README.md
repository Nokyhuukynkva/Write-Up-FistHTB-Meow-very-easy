# Write-Up-FistHTB-Meow-very-easy
Để đi được tới bước này Thì tôi phải cảm mơn Learningvn đã có road map hướng dẫn rất đáng giá
<img width="1305" height="684" alt="image" src="https://github.com/user-attachments/assets/34be0936-a9ec-49a8-863e-0426f6a27f21" />

Mở máy ảo Kali-linux và vào terminal 
Đầu tiên là cài openvpn để kết nối đến thử thách của HTB
<img width="619" height="129" alt="image" src="https://github.com/user-attachments/assets/86e4f84f-36af-4535-879c-4351431f037c" />

Tạo tài khoản Hack The Box và vào Hack labs <img width="204" height="54" alt="image" src="https://github.com/user-attachments/assets/db9a95d1-30a4-443f-a92d-09da0001be84" />

Kết nối openvpn Tải file cấu hình openvpn
<img width="379" height="117" alt="image" src="https://github.com/user-attachments/assets/fec2832d-2e37-4083-acdd-d80ed688ba94" />

Nếu sử dụng Window và chạy bằng máy ảo thì copy file đó sang máy ảo
<img width="765" height="230" alt="image" src="https://github.com/user-attachments/assets/d80f5beb-e16e-4cd5-aaa6-0da84b8c6fe4" />
<img width="702" height="584" alt="image" src="https://github.com/user-attachments/assets/dcd8468b-01af-4fdd-917b-114eeadd665b" />
Khuyến cáo sử dụng Kali-linux cho đầy đủ các chương trình

Tiếp đến là chạy set up openvpn 
<img width="623" height="389" alt="image" src="https://github.com/user-attachments/assets/6c17b807-597e-4fe6-941e-18f6ba4e5a5a" />

Vẫn giữ terminal kết nối đó mở bảng khác

Sử dụng nmap để xem cổng nào có thể khai thác 
lệnh nmap: nmap -sV --top-ports 100 -T4 <ip máy khai thác>
<img width="626" height="259" alt="image" src="https://github.com/user-attachments/assets/260dd525-b7bc-4f51-973a-86428d33668f" />

Phát hiện cổng 23/tcp mở telnet có thể khai thác 
lệnh khai thác: telnet <ip máy khai thác> 23
<img width="253" height="88" alt="image" src="https://github.com/user-attachments/assets/78147dc8-70b5-4769-aff3-d17d4f77a364" />
Kết nối thành công có thể thử các mật khẩu cơ bản (root/root, admin/amin, ubuntu, mint, hoặc user)
để đăng nhập và khai thác flag.txt

<img width="540" height="424" alt="image" src="https://github.com/user-attachments/assets/9fb35deb-5513-4e6f-a312-9e71190fb14d" />

Kết nối thành công bắt đầu khai thác.
<img width="571" height="490" alt="image" src="https://github.com/user-attachments/assets/582b00ba-8546-4593-adf0-2203bbd0d2a7" />

Dùng lệnh ls để xem có những file nào và tìm file flag
<img width="233" height="58" alt="image" src="https://github.com/user-attachments/assets/add3b7e6-958e-4cbe-be88-3a78c96b992d" />

Dùng lệnh: nano để xem flag
<img width="276" height="53" alt="image" src="https://github.com/user-attachments/assets/f01526b5-0e3c-4c76-bf06-db3375544b36" />
Đã tìm được flag
Lưu ý cẩn thận khi copy flag để submit nha coi chừng thiếu chữ


