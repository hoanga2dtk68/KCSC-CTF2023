![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/8cb054de-edc0-4836-9108-07b5fd174d94)

[link down virtual machine](https://drive.google.com/file/d/1uOFf2TN2-y0_mnixzeWQ3q9OaK7WiLd-/view?usp=drivesdk)

Hint 1: nói về việc dăng nhập vào virtual machine qua ssh

Hint 2: nó về CVE đó và cách decrypt nó để lấy máy ảo lúc chưa bị mã hóa

[Link solution](https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-039a)

Đầu tiên chúng ta vào máy ảo và tải file khôi theo hướng dẫn của bài trên và giải mã máy ảo
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/615c9a89-018e-45a2-9873-5cd55623b291)
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/9de4d8e2-dad0-46b1-8703-0f154c4ff593)
Khôi phục thành công máy ảo ban đầu rồi và giờ lấy nó về và chạy trên VMWARE để  lấy flag thôi
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/350e39a8-cdf8-420e-8804-cf82cf4d3919)
Vào máy ảo đọc file secrets.txt và thêm chữ R vào đầu vào decode base64 để lấy flag
![image](https://github.com/hoanga2dtk68/KCSC-CTF2023/assets/110059218/2b65a914-6890-41a1-8505-d0609aff751b)

flag: KCSC{E5%1A2G5-2eC0ve2_EA5y}
