
`Tugas ini merupakan tugas mata kuliah Konsep Jaringan yang dibimbing oleh Bpk. Dr. Ferry Astika Saputra,ST, M.Sc`

# Scenario Switch vs Hub

## Switch

**PC0-PC1** 

https://github.com/Mahargip/Konsep-Jaringan/assets/114201452/60f600ff-784e-4c68-9aba-d69be75313fb


  **PC 0 (192.168.1.2) melakukan ping ke PC 1 (192.168.1.3)**
    
    -   PC 0 memeriksa bahwa PC 1 berada dalam subnet yang sama.
    -   PC 0 mengirimkan permintaan ARP untuk mencari alamat MAC dari PC 1.
    -   PC 1 membalas permintaan ARP dengan alamat MAC-nya.
    -   PC 0 sekarang mengetahui alamat MAC PC 1 dan mengirimkan paket ICMP echo request (ping).
    -   Paket melewati Switch 1 dan mencapai PC 1.
    -   PC 1 membalas dengan paket ICMP echo reply, mengkonfirmasi komunikasi yang berhasil.

**PC0-PC2** 


https://github.com/Mahargip/Konsep-Jaringan/assets/114201452/a3b36c0e-e31d-4ef5-89f7-413316181da7




 **PC 0 (192.168.1.2) melakukan ping ke PC 2 (192.168.6.2)**
    
    -   PC 0 memeriksa bahwa PC 2 berada dalam subnet yang berbeda.
    -   PC 0 mengirimkan permintaan ARP untuk mencari alamat MAC dari antarmuka Router 2 yang terhubung ke Switch 1.
    -   Router 1 membalas permintaan ARP dengan alamat MAC-nya.
    -   PC 0 sekarang mengetahui alamat MAC Router 1 dan mengirimkan paket ICMP echo request.
    -   Paket melewati Switch 1, Router 1, dan Switch 2, mencapai PC 2.
    -   PC 2 membalas dengan paket ICMP echo reply, mengkonfirmasi komunikasi yang berhasil.

**PC0-PC3** 

https://github.com/Mahargip/Konsep-Jaringan/assets/114201452/da09fdc0-4e84-4094-a9e7-7e7761f09e3a





  **PC 0 (192.168.1.2) melakukan ping ke PC 3 (192.168.6.3)**
    
    -   PC 0 memeriksa bahwa PC 3 berada dalam subnet yang berbeda.
    -   PC 0 mengirimkan permintaan ARP untuk mencari alamat MAC dari antarmuka Router 2 yang terhubung ke Switch 2.
    -   Router 1 membalas permintaan ARP dengan alamat MAC-nya.
    -   PC 0 sekarang mengetahui alamat MAC Router 2 dan mengirimkan paket ICMP echo request.
    -   Paket melewati Switch 1, Router 1, dan Switch 2, mencapai PC 3.
    -   PC 3 membalas dengan paket ICMP echo reply, mengkonfirmasi komunikasi yang berhasil.




## Hub

**PC0-PC1** 




https://github.com/Mahargip/Konsep-Jaringan/assets/114201452/710b0fcd-85c6-41c8-88e1-b7edbd53bf11



 **PC 0 (192.168.1.2) melakukan ping ke PC 1 (192.168.1.3)**
    
    -   PC 0 memeriksa bahwa PC 1 berada dalam subnet yang sama.
    -   PC 0 mengirimkan permintaan ARP dalam bentuk broadcast untuk mencari alamat MAC dari PC 1.
    -   Permintaan ARP dan paket data berikutnya dikirimkan ke semua perangkat yang terhubung ke hub.
    -   Baik PC 0 maupun PC 1 menerima permintaan ARP, tetapi hanya PC 1 yang membalas dengan alamat MAC-nya.
    -   PC 0 sekarang mengetahui alamat MAC PC 1 dan mengirimkan paket ICMP echo request.
    -   Paket tersebut melewati Hub 0 dan mencapai PC 1.
    -   PC 1 membalas dengan paket ICMP echo reply, mengkonfirmasi komunikasi yang berhasil.

**PC0-PC2** 



https://github.com/Mahargip/Konsep-Jaringan/assets/114201452/7f2ed67f-c772-4f1f-a5d2-7c0e8c74a37b





  **PC 0 (192.168.1.2) melakukan ping ke PC 2 (192.168.6.2)**
    
    -   PC 0 memeriksa bahwa PC 2 berada dalam subnet yang berbeda.
    -   PC 0 mengirimkan permintaan ARP dalam bentuk broadcast untuk mencari alamat MAC dari antarmuka Router1 yang terhubung ke Hub 0.
    -   Permintaan ARP dan paket data berikutnya dikirimkan ke semua perangkat yang terhubung ke Hub 0.
    -   Baik PC 0 maupun Router1 menerima permintaan ARP, tetapi hanya Router1 yang membalas dengan alamat MAC-nya.
    -   PC 0 sekarang mengetahui alamat MAC Router1 dan mengirimkan paket ICMP echo request.
    -   Paket tersebut melewati Hub 0, Router1, dan Hub 1, mencapai PC 2.
    -   PC 2 membalas dengan paket ICMP echo reply, mengkonfirmasi komunikasi yang berhasil.

**PC0-PC3**




https://github.com/Mahargip/Konsep-Jaringan/assets/114201452/68113c0a-9c27-414a-b15a-f8c2cba2c18f


  **PC 0 (192.168.1.2) melakukan ping ke PC 3 (192.168.6.3)**
    
    -   PC 0 memeriksa bahwa PC 3 berada dalam subnet yang berbeda.
    -   PC 0 mengirimkan permintaan ARP dalam bentuk broadcast untuk mencari alamat MAC dari antarmuka Router1 yang terhubung ke Hub 0.
    -   Permintaan ARP dan paket data berikutnya dikirimkan ke semua perangkat yang terhubung ke Hub 0.
    -   Baik PC 0 maupun Router1 menerima permintaan ARP, tetapi hanya Router1 yang membalas dengan alamat MAC-nya.
    -   PC 0 sekarang mengetahui alamat MAC Router1 dan mengirimkan paket ICMP echo request.
    -   Paket tersebut melewati Hub 0, Router1, dan Hub 1, mencapai PC 3.
    -   PC 3 membalas dengan paket ICMP echo reply, mengkonfirmasi komunikasi yang berhasil.
