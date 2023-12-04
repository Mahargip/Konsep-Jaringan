
`Tugas ini merupakan tugas mata kuliah Konsep Jaringan yang dibimbing oleh Bpk. Dr. Ferry Astika Saputra,ST, M.Sc`

## Traceroute


### Traceroute 1.1.1.1 dan detik.com

![WhatsApp Image 2023-11-07 at 15 31 10_0242fa68](https://github.com/Mahargip/Konsep-Jaringan/assets/114201452/5f3fa639-63c6-4715-b4d5-7993cd2c5f9c)


### Penjelasan
Output dari perintah `traceroute` menunjukkan jalur yang diambil oleh paket data dari komputer Anda menuju tujuan yang ditentukan (dalam kasus ini, tujuan adalah 1.1.1.1 dan detik.com). Berikut adalah penjelasan singkat dari output tersebut:

### Traceroute ke 1.1.1.1:

1. **Hop 1:**
   - Alamat IP: 192.168.1.1 (Gateway lokal Anda)
   - Waktu: 0.124 ms, 0.086 ms, 0.130 ms

2. **Hop 2:**
   - Alamat IP: 10.252.108.212
   - Waktu: 0.189 ms, 0.189 ms, 0.181 ms

3. **Hop 3:**
   - Tidak mendapatkan respons (* * *). Ini bisa terjadi karena host tidak merespons atau paket di-drop oleh firewall.

4. **Hop 4:**
   - Alamat IP: 202.9.85.1 (core-router.pens.ac.id)
   - Waktu: 0.930 ms, 1.024 ms, 1.138 ms

5. **Hop 5:**
   - Alamat IP: 10.252.0.1 (edge-router.pens.ac.id)
   - Waktu: 1.287 ms, 1.305 ms, 1.271 ms

6. **Hop 6:**
   - Alamat IP: 114.4.97.169 (114-4-97-169.resources.indosat.com)
   - Waktu: 2.672 ms, 2.234 ms, 2.352 ms

7. **Hop 7:**
   - Alamat IP: 114.0.78.196 (114-0-78-196.resources.indosat.com)
   - Waktu: 23.153 ms, 23.321 ms, 23.989 ms

8. **Hop 8:**
   - Tidak mendapatkan respons (* * *). Kembali, mungkin ada kebijakan firewall atau host yang tidak merespons.

9. **Hop 9:**
   - Alamat IP: 162.158.168.2 dan 162.158.160.19
   - Waktu: 25.339 ms, * (TTL habis), 23.773 ms

10. **Hop 10:**
   - Alamat IP: 1.1.1.1 (one.one.one.one)
   - Waktu: 24.495 ms, * (TTL habis), 24.816 ms

### Traceroute ke detik.com:

1. **Hop 1:**
   - Alamat IP: 192.168.1.1 (Gateway lokal Anda)
   - Waktu: 0.128 ms, 0.097 ms, 0.089 ms

2. **Hop 2:**
   - Alamat IP: 10.252.108.212
   - Waktu: 0.199 ms, 0.182 ms, 0.160 ms

3. **Hop 3:**
   - Alamat IP: 103.24.56.241 (241.56.pens.ac.id)
   - Waktu: 0.569 ms, 0.548 ms, tidak mendapatkan respons (* * *)

4. **Hop 4:**
   - Alamat IP: 202.9.85.1 (core-router.pens.ac.id)
   - Waktu: 1.105 ms, 1.101 ms, 1.092 ms

5. **Hop 5:**
   - Alamat IP: 10.252.0.1 (edge-router.pens.ac.id)
   - Waktu: 1.070 ms, 1.058 ms, 1.035 ms

6. **Hop 6:**
   - Alamat IP: 124.195.39.3 (124-195-39-3.resources.indosat.com)
   - Waktu: 12.931 ms, 12.983 ms, 13.120 ms

7. **Hop 7:**
   - Tidak mendapatkan respons (* * *), kemungkinan firewall atau host tidak merespons.

8. **Hop 8:**
   - Alamat IP: 218.100.36.9
   - Waktu: 14.291 ms, 13.195 ms, 13.171 ms

9. **Hop 9:**
   - Alamat IP: 203.190.242.211 (s2-211-242.190.203.detik.com)
   - Waktu: 12.974 ms, 12.933 ms, 12.919 ms

Jadi, hasil `traceroute` memberikan gambaran tentang perjalanan paket dari sumber ke tujuan melalui berbagai hop di jaringan. Beberapa hop mungkin tidak merespons tergantung pada kebijakan firewall atau pengaturan di perangkat tersebut.
