===================================================
 TIC-TAC-TOE GAME - HUONG DAN BIEN DICH VA CHAY
===================================================

1. YEU CAU
----------
  - Trinh bien dich: g++ phien ban >= 15.2.0 (ho tro C++20)
  - He dieu hanh: Windows

2. BIEN DICH
------------
  Mo terminal (Command Prompt / PowerShell) tai thu muc chua file game.cpp.

  Lenh co ban:
    g++ -std=c++20 game.cpp -o game.exe

  Bat canh bao:
    g++ -std=c++20 -Wall -Wextra game.cpp -o game.exe

  Ban debug:
    g++ -std=c++20 -Wall -Wextra -g game.cpp -o game.exe

  Hoac su dung VS Code: Ctrl + Shift + B (can cau hinh tasks.json truoc).

3. CHAY CHUONG TRINH
---------------------
  a) Che do tuong tac (mac dinh):
       game.exe

     Chuong trinh se hien menu de nguoi choi chon:
       - Kich thuoc ban co (toi da 12x12)
       - Dieu kien thang (so quan lien tiep)
       - Che do choi: PvP / PvE / EvE
       - Do kho bot (neu co bot): Easy / Medium / Hard

  b) Che do cham diem (judge mode):
       game.exe --judge --input input1.txt

     Doc du lieu tu file, khong hien giao dien, chi xuat ket qua.

4. CAC TUY CHON DONG LENH
--------------------------
  --judge, -j      Bat che do cham diem (tat giao dien)
  --input, -i      Duong dan file input (dung voi --judge)
  --log,   -l      Duong dan file log (mac dinh: log.txt)
  --help,  -h      Hien huong dan su dung

5. VI DU
--------
  game.exe                              Choi tuong tac binh thuong
  game.exe -j -i input1.txt            Chay voi test case 1
  game.exe -j -i input2.txt -l out.txt Chay test case 2, ghi log ra out.txt

===================================================
