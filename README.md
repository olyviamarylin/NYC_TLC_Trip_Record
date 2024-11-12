# NYC_TLC_Trip_Record

**LATAR BELAKANG**

Sebuah perusahaan taksi/rental mobil di New York City menghadapi tantangan untuk memaksimalkan profit dalam industri yang sangat kompetitif. Dengan munculnya layanan transportasi daring, perusahaan-perusahaan taksi tradisional harus menyesuaikan strategi mereka agar tetap relevan dan menguntungkan bagi perusahaan. Berdasarkan data yang disediakan oleh New York City Taxi and Limousine Commission (TLC), terdapat beberapa aspek utama yang memengaruhi profitabilitas perusahaan taksi, seperti metode pembayaran, jam ramai, serta jarak dan zona perjalanan.
Data tersebut dapat  dimanfaatkan untuk menganalisis tren pendapatan dan mengidentifikasi faktor-faktor yang paling berpengaruh terhadap profit. Pemahaman yang mendalam atas data ini penting untuk menemukan peluang peningkatan profit, terutama pada masa-masa tertentu, seperti jam sibuk atau musim liburan, di mana permintaan akan layanan taksi/rental mobil meningkat.
Dengan memetakan pola permintaan, perusahaan dapat menempatkan armada mereka di area dengan permintaan tinggi sehingga meningkatkan kemungkinan mendapatkan penumpang dan memaksimalkan penggunaan armada. Strategi pemasaran dan program loyalitas juga dapat diperkuat untuk menarik pelanggan dan mempertahankan mereka dalam jangka panjang. Dengan pendekatan berbasis data ini, perusahaan dapat mengambil keputusan yang lebih informasional dan berbasis bukti untuk meningkatkan profitabilitas di pasar yang sangat kompetitif.


**TUJUAN**

untuk menganalisa peluang pada perusahaan, manager operasional dibantu oleh seorang data analyst melakukan evaluasi pada data yang telah dimiliki sebelumnya. adapun tujuan yang akan di analisa adalah:

Memaksimalkan penyewaan armada yang dimiliki. Apakah terdapat jam ramai terkait banyaknya armada yang di sewa?
Berdasarkan data yg dimiliki, Tipe Perjalanan dan Metode Pembayaran apa yang paling di minati oleh pelanggan?
Zona manakah yang paling ramai?

**DATA SET ORIGINAL**
![image](https://github.com/user-attachments/assets/b58e5c9a-d216-40e0-bae0-c6f3acf18f86)
![image](https://github.com/user-attachments/assets/78692d67-1c15-4beb-bb10-6bf62d16ef7b)

**DESKRIPSI KOLOM**

Data berikut berisi tentang:

1. **VendorID**: Kode yang menunjukkan penyedia LPEP (sistem perekaman perjalanan) yang menyediakan data ini.
   - 1 = Creative Mobile Technologies, LLC.
   - 2 = VeriFone Inc.

2. **lpep_pickup_datetime**: Tanggal dan waktu saat meteran taksi mulai berjalan, menandai awal perjalanan.

3. **lpep_dropoff_datetime**: Tanggal dan waktu saat meteran taksi berhenti, menandai akhir perjalanan.

4. **Passenger_count**: Jumlah penumpang di kendaraan, yang dimasukkan oleh pengemudi.

5. **Trip_distance**: Jarak tempuh perjalanan dalam mil, yang dilaporkan oleh meteran taksi.

6. **PULocationID**: ID zona lokasi TLC di mana meteran taksi diaktifkan atau tempat penjemputan.

7. **DOLocationID**: ID zona lokasi TLC di mana meteran taksi dihentikan atau tempat tujuan.

8. **RateCodeID**: Kode tarif yang berlaku pada akhir perjalanan.
   - 1 = Tarif standar
   - 2 = JFK
   - 3 = Newark
   - 4 = Nassau atau Westchester
   - 5 = Tarif yang dinegosiasikan
   - 6 = Perjalanan grup

9. **Store_and_fwd_flag**: Tanda yang menunjukkan apakah catatan perjalanan disimpan sementara di memori kendaraan sebelum dikirim ke penyedia karena tidak ada koneksi ke server.
   - Y = Perjalanan disimpan dan diteruskan kemudian
   - N = Perjalanan tidak disimpan sementara

10. **Payment_type**: Kode yang menunjukkan cara pembayaran yang dilakukan oleh penumpang.
    - 1 = Kartu kredit
    - 2 = Tunai
    - 3 = Tanpa biaya
    - 4 = Perselisihan
    - 5 = Tidak diketahui
    - 6 = Perjalanan dibatalkan

11. **Fare_amount**: Biaya perjalanan berdasarkan jarak dan waktu yang dihitung oleh meteran.

12. **Extra**: Biaya tambahan, termasuk biaya tambahan jam sibuk ($0.50 atau $1 untuk jam sibuk dan tengah malam).

13. **MTA_tax**: Pajak MTA sebesar $0.50 yang diterapkan secara otomatis berdasarkan tarif meter yang digunakan.

14. **Improvement_surcharge**: Biaya peningkatan sebesar $0.30 yang dikenakan pada perjalanan yang dimulai sejak tahun 2015.

15. **Tip_amount**: Jumlah tip yang diberikan, secara otomatis diisi untuk pembayaran dengan kartu kredit (tidak termasuk tip tunai).

16. **Tolls_amount**: Total biaya tol yang dibayar dalam perjalanan.

17. **Total_amount**: Total biaya yang dibebankan kepada penumpang (tidak termasuk tip tunai).

18. **Trip_type**: Kode yang menunjukkan apakah perjalanan adalah "street-hail" (perjalanan yang dipanggil langsung di jalan) atau "dispatch" (pesanan taksi yang diatur sebelumnya).
    - 1 = Street-hail
    - 2 = Dispatch

19. **congestion_surcharge**: biaya tambahan kemacetan yang dikenakan pada perjalanan taksi, Besarnya biaya ini adalah sebesar $2.75 untuk taksi biasa dan sekitar $2.50 untuk kendaraan sewa lainnya.

**VISUALISASI DATA**
![image](https://github.com/user-attachments/assets/47313d01-01a2-4c86-97a1-61907579e948)

**KESIMPULAN**

Dari analisa yang telah dilakukan, maka perusahaan dapat mengambil kesimpulan untuk melakukan langkah-langkah apa yang akan dilakukan untuk selanjutnya, yaitu:

1. Memaksimalkan armada yang dimiliki dengan mengetahui zona mana yang ramai picup yaitu zona 74, 75, 95, 41, dst. perusahaan dapat memetakan armada di area tersebut dan di jam 15 sampai jam 18
2. metode pembayaran yang paling diminati oleh customer adalah dengan menggunakan kartu kredit, perusahaan dapat melakukan pengecekan rutin pada mesin untuk penggunaan kartu kredit yang tersedia dalam mobil atau pada handphone driver dipastikan selalu bisa di gunakan untuk menghindari customer tidak jadi naik armada yg dimiliki karena tidak bisa melakukan pembayaran menggunakan kartu kredit
3. melakukan penghindara pada zona macet yang tidak ramai, jika armada di petakan di zona macet namun tidak ramai penumpang maka akan menimbulkan kerugian perusahaan karena memakan banyak bahan bakar kendaraan

