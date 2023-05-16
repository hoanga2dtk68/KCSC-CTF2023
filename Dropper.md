![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/b8cbf519-e218-4c4e-857a-d1d56d4480d7)

Mount ổ lên máy và xem log xem có gì không
Đồng thời đầu bài cũng là một gợi ý rất quan trọng 
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/408405a1-4a8f-42c0-85e4-f745db723ff7)
xem log powershell thì cũng thấy có nhiều các script khác nhau được cảnh báo và thông báo đang bbị remote từ xa
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/1e7527dc-8775-4a3b-8ec5-7d6c4fbba0ee)
cho thấy đây cũng là một trojan đúng theo tên của đầu bài
Sau khi tìm nguồn gốc của trojan thì nó sinh ra từ chrome

![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/a24c8b98-0d46-45e9-b0ba-1f802c7a7c5e)
sau khi lấy được file này ra thì check đây là một file cab chứa file ps chạy bên trong
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/342e7eee-6018-4ab4-a2ca-4338ac67b3e8)
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/c788fa13-509f-47ef-a09e-4bf7017ed6a7)
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/dd23753d-5182-4311-9654-15caefd69ee0)
sửa thực thi thành echo để xem thực thi tiếp như thế nào
sau khi thực hiện một lúc thì cuối cùng đã đến đích
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/f56877db-3e79-484e-adac-d1427898bf69)
đến cuối đọc thì có thấy giải mã và phải đúng computername mới lưu vào trong nên ném lên cyberchef để giải mã
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/16af543d-fe52-4001-a880-269d63b0d894)
Thấy header rất quen đây là jpg hay jpeg lưu về và đổi extension thôi là nhận được flag
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/9a3b15e4-5cbc-454b-8c92-9909cb3ee539)
flag: KCSC{Som3one's_thr0ugh1s_KMA_don't_have_researcher?}
