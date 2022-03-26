github URL： https://github.com/sssh311318/hw2

此次作業是 把Gaussian blur 和 testbench 透過TLM bus 連接。
我是參考lab4 的範例code 作為基礎更改成Gaussian blur的filter,
TLM的傳輸方法和lab04相同，testbench 的initiator 連到 bus target，
bus的initiator 連到 Gaussian blur 的 target ,同樣的memory map address的設定，
與sobel filter不同的地方是，我的mask 只有 一個 3*3 的 matrix ，所以我在計算convolution的時候有做修改。
我還有在testbench.cpp裡面，我將原本判斷black和white的部分作修改，把threshold移除掉，直接將total輸出回原本RGB的位置，所以圖片輸出才會是灰階。
在做HW2的時候，我大部分時間都花在了解LAB03和LAB04上面，實作上花較少的時間。
在這次的作業我學到了TLM是如何做交換的，還有透過SIMPLE BUS 可以跟不同的MODULE做資料交換。



