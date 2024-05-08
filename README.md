## 2.1. Original code of broadcast chat.
![alt text](image-2.png)
![alt text](image-3.png)
![alt text](image-4.png)
![alt text](image-5.png)
<br>
membuka 4 terminal dan menjalan kan 1 server dan 3 client. <br>
jalankan server dengan ```cargo run --bin server``` <br>
jalankan client dengan ```cargo run --bin client ``` <br>
Gambar tersebut memunculkan bahwa setiap client menerima ketiga message yang dikirimkan ke server.

## 2.2 Modifying the websocket port
![alt text](image.png)
![alt text](image-1.png)
![alt text](image-6.png)
![alt text](image-7.png)
<br>
Pada gambar di atas saya merubah port pada server.rs dan juga client.rs makanya mereka dapat menerima message. Namun jika pada client.rs tidak diganti maka akan memunculkan error karena otomatis disconnect dengan server karena alamat port yang berbeda.

## 2.3 Small changes. Add some information to client
![alt text](image-8.png)
![alt text](image-9.png)
![alt text](image-10.png)
![alt text](image-11.png)
<br>
Dengan modifikasi kecil tersebut, dapat dimunculkan dari IP mana message tersebut dikirimkan. Ini dilakukan dengan menambahkan pada bcast.tx.