#WIDE
Sau khi giải nén ta có 2 file, đưa file vào detect it easy:
![image](https://github.com/NamDT5125/ctf/assets/69895129/ff3e622e-b4e2-442b-8403-4704c07b854d)
![image](https://github.com/NamDT5125/ctf/assets/69895129/b7592771-ffb7-4278-9ded-8f59aa109134)
![image](https://github.com/NamDT5125/ctf/assets/69895129/6a12fade-dbe9-47e7-a175-e8119aa20371)
Ta thấy 1 file là binary và 1 file là elf64 
Sau khi chạy file ta có:
![image](https://github.com/NamDT5125/ctf/assets/69895129/1750706f-dd05-41fa-b4cd-2042d2e33344)
Sau khi chạy, ta nhập vào các số, đến số thứ 6 thì yêu cầu nhập key
![image](https://github.com/NamDT5125/ctf/assets/69895129/a6edf826-7104-4457-9490-98e59f2e91c3)
Mở IDA lên để dịch ngược:
![image](https://github.com/NamDT5125/ctf/assets/69895129/6da43391-5835-40a5-878a-e11adee42bfd)
Vì sau khi nhập key nó ra incorrect nên ta tìm trong strings và tìm vào code:
![image](https://github.com/NamDT5125/ctf/assets/69895129/94b6b30f-4250-4c02-bb88-e9c4d923dbb9)
Ta thấy ở đây nó so sánh giá trị s1 và s2 mà s1 là phần nhập key nên ta check thử s2:
![image](https://github.com/NamDT5125/ctf/assets/69895129/1c6dbd17-0b42-47da-bb11-97dadbe4022c)
![image](https://github.com/NamDT5125/ctf/assets/69895129/27bbdec3-0ca9-491a-b311-635f1e99b87c)
Key là `sup3rs3cr3tw1d3 `
![image](https://github.com/NamDT5125/ctf/assets/69895129/b1d62707-43af-44d5-a4fe-40fca24271ec)
`HTB{som3_str1ng5_4r3_w1d3}`
