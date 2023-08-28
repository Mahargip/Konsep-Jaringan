<h1>Praktikum Wireshark menggunakan Sample</h1>

</br>

<p>Nama  : Mahargi Anugerahwan Pamungkas</p>
<p>Kelas : 2 D4 IT A</p>
<p>NRP   : 3122600012</p>

</br>

<p>Pada percobaan ini, kita menggunakan sample http.cap yang sudah kita download.</p>
<div style="text-align:center">
  <img src="../assets/wireshark-1.png"/>
</div>

</br>

<p>Untuk melihat seluruh aliran data dari sesi HTTP (HyperText Transfer Protocol) yang ditangkap dalam paket jaringan, kita dapat menggunakan fitur "Follow HTTP Stream". Ini membantu untuk melihat permintaan dan respons HTTP secara keseluruhan dalam konteks yang lebih mudah dibaca</p>
<div style="text-align:center">
  <img src="../assets/wireshark-2.png"/>
</div>

</br>

<p>Warna merah merupakan "request". ni mencakup permintaan yang dikirim oleh klien (seperti browser) ke server. Anda akan melihat detail seperti metode (GET, POST, dll.), URI, dan header permintaan.</p>
<div style="text-align:center">
  <img src="../assets/wireshark-4.png"/>
</div>

<br>

<p>Sedangkan warna biru merupakan "response". Ini mencakup balasan yang dikirim oleh server kepada klien sebagai tanggapan terhadap permintaan. Anda dapat melihat kode status HTTP, header respons, dan body data (jika ada).</p>
<div style="text-align:center">
  <img src="../assets/wireshark-5.png"/>
</div>

<br>

<p>Berikut jika keduanya digabungkan</p>
<div style="text-align:center">
  <img src="../assets/wireshark-3.png"/>
</div>

<br>

<p>Lalu kita juga dapat melihat berbagai informasi dari source yang kita inginkan. Semisalnya kita dapat melihat Source Port, dan Destination Portnya (Ditunjukkan bahwa Destination Portnya adalah 80 yang menandakan standar port untuk Web Server.)</p>
<div style="text-align:center">
  <img src="../assets/wireshark-6.png"/>
  <img src="../assets/wireshark-7.png">
</div>

<br>

