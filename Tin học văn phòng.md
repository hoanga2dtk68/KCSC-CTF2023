![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/f530ac27-08d2-4c79-80a4-415cf2721768)

Đầu tiên ném lên Virustotal thì có phát hiện có mã độc thì chắc đây là dạng VBA macros
dùng oletools check thì thấy flag có 2 phần: KCSC{H1_1m_sUcky_+$phlac}
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/5402ee7a-cd3f-4bcc-b19b-254f652951e8)
Giờ thì cần tìm giá trị của biến phlac để nhận flag hoàn chỉnh
Mở file docm bằng máy ảo và cho thực thi được ẩn lên, sau khi chạy xong powershell thì xuất hiện một thông báo

![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/b52a92ca-61df-4445-bc8a-cc09c85ef160)
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/3f6cdc8f-6f58-4091-8af5-2b87e0076dd2)
Mình đã chuyển tiền đến nhưng không nhận được gì
Vào log Powershell để xem từ file docm đã thực thi những gì trên máy

![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/2e7baeaf-e2ef-4674-8a7c-54c3e8abee6e)
thấy có thực thi ném lên powershelldecoder thì nhận được biến phlac
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/bb989d2d-b9ea-4b4c-9213-be6a85d2b4ba)
$phlac = Tr0ll_m4lw@r3_y0u_g0t_m3_ah1Hi}
flag: KCSC{H1_1m_sUcky_Tr0ll_m4lw@r3_y0u_g0t_m3_ah1Hi}
