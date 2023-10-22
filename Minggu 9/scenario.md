# Scenario Switch vs Hub

## Switch

**PC0-PC1**

*CLICK IMAGE FOR VIDEO*

[<img src="../assets/switchlogo.png" width="600" height="300"
/>](https://www.youtube.com/embed/7eLdtQx9q40)


  **PC 0 (192.168.1.2) melakukan ping ke PC 1 (192.168.1.3)**
    
    -   PC 0 memeriksa bahwa PC 1 berada dalam subnet yang sama.
    -   PC 0 mengirimkan permintaan ARP untuk mencari alamat MAC dari PC 1.
    -   PC 1 membalas permintaan ARP dengan alamat MAC-nya.
    -   PC 0 sekarang mengetahui alamat MAC PC 1 dan mengirimkan paket ICMP echo request (ping).
    -   Paket melewati Switch 1 dan mencapai PC 1.
    -   PC 1 membalas dengan paket ICMP echo reply, mengkonfirmasi komunikasi yang berhasil.

**PC0-PC2**
<iframe width="600" height="300" src="https://www.youtube.com/embed/G49Zi6WcPmI" title="switch pc0-pc2" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

 **PC 0 (192.168.1.2) melakukan ping ke PC 2 (192.168.6.2)**
    
    -   PC 0 memeriksa bahwa PC 2 berada dalam subnet yang berbeda.
    -   PC 0 mengirimkan permintaan ARP untuk mencari alamat MAC dari antarmuka Router 2 yang terhubung ke Switch 1.
    -   Router 1 membalas permintaan ARP dengan alamat MAC-nya.
    -   PC 0 sekarang mengetahui alamat MAC Router 1 dan mengirimkan paket ICMP echo request.
    -   Paket melewati Switch 1, Router 1, dan Switch 2, mencapai PC 2.
    -   PC 2 membalas dengan paket ICMP echo reply, mengkonfirmasi komunikasi yang berhasil.

**PC0-PC3**
<iframe width="600" height="300" src="https://www.youtube.com/embed/qBt0-g1KnHU" title="switch pc0-pc3" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

  **PC 0 (192.168.1.2) melakukan ping ke PC 3 (192.168.6.3)**
    
    -   PC 0 memeriksa bahwa PC 3 berada dalam subnet yang berbeda.
    -   PC 0 mengirimkan permintaan ARP untuk mencari alamat MAC dari antarmuka Router 2 yang terhubung ke Switch 2.
    -   Router 1 membalas permintaan ARP dengan alamat MAC-nya.
    -   PC 0 sekarang mengetahui alamat MAC Router 2 dan mengirimkan paket ICMP echo request.
    -   Paket melewati Switch 1, Router 1, dan Switch 2, mencapai PC 3.
    -   PC 3 membalas dengan paket ICMP echo reply, mengkonfirmasi komunikasi yang berhasil.




## Hub

**PC0-PC1**
<iframe width="600" height="300" src="https://www.youtube.com/embed/muCSgqRCRAc" title="Hub pc0-pc1" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

 **PC 0 (192.168.1.2) melakukan ping ke PC 1 (192.168.1.3)**
    
    -   PC 0 memeriksa bahwa PC 1 berada dalam subnet yang sama.
    -   PC 0 mengirimkan permintaan ARP dalam bentuk broadcast untuk mencari alamat MAC dari PC 1.
    -   Permintaan ARP dan paket data berikutnya dikirimkan ke semua perangkat yang terhubung ke hub.
    -   Baik PC 0 maupun PC 1 menerima permintaan ARP, tetapi hanya PC 1 yang membalas dengan alamat MAC-nya.
    -   PC 0 sekarang mengetahui alamat MAC PC 1 dan mengirimkan paket ICMP echo request.
    -   Paket tersebut melewati Hub 0 dan mencapai PC 1.
    -   PC 1 membalas dengan paket ICMP echo reply, mengkonfirmasi komunikasi yang berhasil.

**PC0-PC2**
<iframe width="600" height="300" src="https://www.youtube.com/embed/T_i8JdH4ziA" title="hub pc0-pc2" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

  **PC 0 (192.168.1.2) melakukan ping ke PC 2 (192.168.6.2)**
    
    -   PC 0 memeriksa bahwa PC 2 berada dalam subnet yang berbeda.
    -   PC 0 mengirimkan permintaan ARP dalam bentuk broadcast untuk mencari alamat MAC dari antarmuka Router1 yang terhubung ke Hub 0.
    -   Permintaan ARP dan paket data berikutnya dikirimkan ke semua perangkat yang terhubung ke Hub 0.
    -   Baik PC 0 maupun Router1 menerima permintaan ARP, tetapi hanya Router1 yang membalas dengan alamat MAC-nya.
    -   PC 0 sekarang mengetahui alamat MAC Router1 dan mengirimkan paket ICMP echo request.
    -   Paket tersebut melewati Hub 0, Router1, dan Hub 1, mencapai PC 2.
    -   PC 2 membalas dengan paket ICMP echo reply, mengkonfirmasi komunikasi yang berhasil.

**PC0-PC3**
<iframe width="600" height="300" src="https://www.youtube.com/embed/Pp9ysNTPoIs" title="hub pc0-pc3" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

  **PC 0 (192.168.1.2) melakukan ping ke PC 3 (192.168.6.3)**
    
    -   PC 0 memeriksa bahwa PC 3 berada dalam subnet yang berbeda.
    -   PC 0 mengirimkan permintaan ARP dalam bentuk broadcast untuk mencari alamat MAC dari antarmuka Router1 yang terhubung ke Hub 0.
    -   Permintaan ARP dan paket data berikutnya dikirimkan ke semua perangkat yang terhubung ke Hub 0.
    -   Baik PC 0 maupun Router1 menerima permintaan ARP, tetapi hanya Router1 yang membalas dengan alamat MAC-nya.
    -   PC 0 sekarang mengetahui alamat MAC Router1 dan mengirimkan paket ICMP echo request.
    -   Paket tersebut melewati Hub 0, Router1, dan Hub 1, mencapai PC 3.
    -   PC 3 membalas dengan paket ICMP echo reply, mengkonfirmasi komunikasi yang berhasil.
