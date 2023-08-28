<h1>Mengapa FTP dapat Memakai TCP/UDP</h1>

</br>

<p>Nama  : Mahargi Anugerahwan Pamungkas</p>
<p>Kelas : 2 D4 IT A</p>
<p>NRP   : 3122600012</p>

</br>

<div style="text-align:center">
  <img src="../assets/udp-tcp.png"/>
</div>

<p>Protokol FTP (File Transfer Protocol) secara tradisional menggunakan TCP (Transmission Control Protocol) untuk koneksi kontrol dan transfer data. Namun, beberapa implementasi atau variasi dari FTP memungkinkan penggunaan protokol UDP (User Datagram Protocol) dalam beberapa situasi tertentu. Ini dapat terjadi karena perbedaan tujuan dan sifat masing-masing protokol:</p>

</br>

<ol>
  <li>
    TCP (Transmission Control Protocol)
    <div>
      <ul>
        <li>Keandalan: TCP menjamin pengiriman data yang andal, terurut, dan tanpa kerusakan. Ini sangat cocok untuk situasi di mana integritas data dan pengiriman yang akurat diperlukan, seperti saat mengunduh atau mengunggah file.</li>
        <li>Koneksi Berbasis: TCP menggunakan pendekatan koneksi berbasis, di mana ada proses pembukaan, pemeliharaan, dan penutupan koneksi antara pengirim dan penerima.</li>
      </ul>
    </div>
  </li>
  </br>
  <li>
    UDP (User Diagram Protocol)
    <div>
      <ul>
        <li>Non-berbasis Koneksi: UDP tidak memiliki mekanisme pembukaan atau pemeliharaan koneksi. Ini memungkinkan pengiriman data lebih cepat, tetapi tanpa jaminan pengiriman yang andal.</li>
        <li>Kehilangan Paket: UDP tidak memiliki mekanisme untuk menggantikan paket data yang hilang, sehingga cocok untuk aplikasi yang lebih toleran terhadap hilangnya beberapa data.</li>
      </ul>
    </div>
  </li>
</ol>

<br>

<p>Beberapa implementasi atau variasi dari FTP mungkin menggunakan protokol UDP dalam beberapa situasi karena beberapa alasan:</p>

<br>

<ol>
  <li>Kecepatan: 
    <div>
      UDP dapat digunakan untuk transfer data yang lebih cepat, karena tidak ada overhead pembukaan dan pemeliharaan koneksi seperti pada TCP.
    </div>
  </li>
  <li>
    <div>
      Multicast atau Broadcast: UDP sering digunakan untuk pengiriman ke banyak penerima sekaligus dalam mode multicast atau broadcast.
    </div>
  </li>
  <li>
    <div>
      Streaming: Jika FTP digunakan untuk tujuan streaming data, misalnya video atau audio, UDP dapat berguna karena data yang diterima lebih cepat, bahkan jika beberapa paket hilang.
    </div>
  </li>
</ol>

<br>

<p>
Namun, penting untuk diingat bahwa menggunakan UDP dalam protokol transfer file seperti FTP dapat mengakibatkan hilangnya keandalan dan akurasi dalam pengiriman data. UDP lebih cocok untuk aplikasi yang lebih toleran terhadap hilangnya beberapa data atau untuk situasi di mana kecepatan pengiriman lebih diutamakan daripada keandalan.
</p>