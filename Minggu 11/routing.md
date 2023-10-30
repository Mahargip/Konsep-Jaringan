# Routing

*Routing* dibagi menjadi 2, yaitu *Static* dan *Dynamic*.
1. **Static Routing**:

-   Static routing melibatkan konfigurasi manual dan statis dari tabel routing di perangkat jaringan. Ini berarti administrator jaringan harus secara eksplisit menentukan rute lalu lintas, yaitu jalur yang akan diikuti oleh paket data dari satu perangkat atau subnet ke perangkat atau subnet lain.
-   Tabel routing statis harus diperbarui secara manual setiap kali ada perubahan dalam topologi jaringan. Ini bisa menjadi pilihan yang baik untuk jaringan kecil yang memiliki sedikit perubahan dalam struktur atau rute.
-   Keuntungan dari static routing adalah bahwa ini sederhana, efisien, dan dapat memberikan kontrol yang lebih besar atas rute lalu lintas. Namun, itu tidak efisien untuk jaringan besar atau yang berubah secara dinamis.

2. **Dynamic Routing**:

-   Dynamic routing, sebaliknya, melibatkan penggunaan protokol routing yang memungkinkan perangkat jaringan untuk berkomunikasi satu sama lain dan secara otomatis mengganti tabel routing saat terjadi perubahan dalam jaringan.
-   Protokol routing dinamis seperti RIP (Routing Information Protocol), OSPF (Open Shortest Path First), dan BGP (Border Gateway Protocol) digunakan untuk mengirim informasi tentang rute yang ada dan memungkinkan perangkat jaringan untuk secara otomatis memutakhirkan tabel routing mereka.
-   Dynamic routing lebih cocok untuk jaringan yang besar dan kompleks, di mana perubahan dalam topologi jaringan atau kegagalan perangkat harus diatasi dengan cepat. Hal ini juga memungkinkan untuk membagi beban lalu lintas secara efisien di seluruh jaringan.

Pada *Routing* terdapat sebutan *Edge Router* dan *Core Router*. 
1. **Edge Router**:

-   Edge router, juga dikenal sebagai router perbatasan atau router akses, berada di tepi (edge) jaringan dan menghubungkan jaringan lokal dengan jaringan luar, seperti Internet atau jaringan lainnya.
-   Peran utama edge router adalah menghubungkan perangkat dalam jaringan lokal Anda dengan sumber daya di luar jaringan, seperti server web, layanan cloud, atau jaringan lain melalui protokol seperti BGP, OSPF, atau RIP.
-   Edge router juga bertanggung jawab untuk mengelola masalah keamanan, seperti firewalling, NAT (Network Address Translation), dan implementasi kebijakan keamanan.

2. **Core Router**:

-   Core router, juga dikenal sebagai router inti, berada di dalam jaringan dan digunakan untuk menghubungkan jaringan-jaringan dalam infrastruktur jaringan yang lebih besar.
-   Core router bertanggung jawab untuk mengarahkan lalu lintas data di dalam jaringan dan memutuskan jalur yang paling efisien untuk mengirim data antara berbagai jaringan atau subnet.
-   Mereka biasanya terletak di pusat jaringan dan digunakan untuk mengelola lalu lintas data dalam skala yang sangat besar. Core router harus memiliki kapasitas pemrosesan yang tinggi dan sangat andal.


Router PENS :
![image](https://github.com/Mahargip/Konsep-Jaringan/assets/114201452/c9ae1f89-2712-4809-bda3-caf47927a89f)

