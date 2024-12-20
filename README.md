<h2 align="center">
<p align="center"><img src="https://raw.githubusercontent.com/kalenderjawa/pustaka/master/images/kj_v2.png" width="50%" alt="sengkala"></p>
</h2>

## Kalender Jawa

Kalender Jawa adalah sistem kalender berbasis bulan. Masyarakat Jawa telah menggunakannya untuk berbagai keperluan dalam kehidupan sehari-hari sejak abad ke-14 hingga sekarang.

## Pustaka 

[Pustaka](https://github.com/kalenderjawa/pustaka) adalah nama perpustakaan npm JavaScript untuk Kalender Jawa.

## API

API ini mudah digunakan. Sebagai contoh, jika Anda ingin mengetahui rumus matematis untuk bulan `romadon` pada tahun Jawa 1952:

```js
KalenderJawa.cariRumusAbadiAwalBulanTahunJawa('romadon', 1952).then(data => {
  console.log(`${data.rumus.wulan.wulan}_${data.rumus.dino}_${data.rumus.pasaran}`)
  // romadon_7_4 (don tu pat)
})
```

## Sejarah

Kalender atau Penanggalan Jawa merupakan penanggalan yang dibawa oleh para leluhur Jawa dan kemudian diolah lebih lanjut oleh para Wali. Sebelum masa para Wali, para leluhur Jawa telah memakai penanggalan berdasarkan matahari atau Saka dan juga berdasarkan bulan.

Dalam perkembangan selanjutnya, para Wali yang berkolaborasi dengan para leluhur bangsa Jawa menghasilkan Penanggalan Jawa yang baru berdasarkan pergerakan bulan. Penanggalan Jawa baru ini sudah umum dipakai sejak Raden Patah menjadi Sultan Demak yang pertama.

Momen ketika Raden Patah menjadi sultan pertama di Demak ditandai dengan *Sengkalan* atau *Candra Sengkala*:

### *Catur Ilang Sucining Ratu*

Sengkalan tersebut menandakan tahun 1404 Saka (887 H, 1482 M) atau 4 tahun setelah runtuhnya Majapahit.

> *Candra Sengkala* atau *Sengkalan* adalah cara orang Jawa mengingat momen tahun dalam bentuk kalimat. Contoh terkenal adalah runtuhnya Majapahit: "Sirna ilang Kertaning Bumi" (1400 Jawa). *Sengkalan* adalah kalender lunar yang sudah lama dipakai sebelum masa para wali [sumber](https://www.caknun.com/2019/kalender-jowo-digowo-kalender-arab-digarap-kalender-barat-diruwat).

Pada masa Sultan Agung, Kalender Jawa diresmikan sebagai kalender kerajaan pada Jumat Legi, 1 Sura 1555 (1 Muharram 1043 H, 8 Juli 1633 M). Kalender ini berlaku di seluruh Pulau Jawa kecuali Banten, Blambangan, dan Madura.

> Para leluhur bangsa Indonesia sebenarnya lebih cepat dalam merumuskan sistem kalender, yaitu lebih dari 100 tahun sebelum Kalender Gregorian diresmikan (1582 M).

## Sistematis

Kalender Jawa sangat kompleks, tetapi dalam *Pustaka Kalender Jawa*, hanya konsep-konsep dasar yang diimplementasikan. Aturan dasar yang menjadi acuan:

- Menggunakan sistem 7 hari (*saptawara*), sama dengan kalender Masehi.
- Menggunakan sistem 5 hari (*pancawara*), dikenal dengan Pasaran.
- Mempunyai siklus 8 tahunan (*windu*).
- Koreksi keberulangan dilakukan setiap 120 tahun (15 *windu*), dikenal sebagai **Salin Kurup** atau **Ganti Kurup** (penambahan 1 hari tiap 120 tahun).

### Hari (*Dinten*/Dino)

Seperti kalender Masehi, Kalender Jawa membagi hari menjadi 7:

| Urutan | Dinten | Hari (Masehi) |
|--------|--------|---------------|
| 1      | Senen  | Senin         |
| 2      | Selasa | Selasa        |
| 3      | Rebo   | Rabu          |
| 4      | Kemis  | Kamis         |
| 5      | Jemah  | Jumat         |
| 6      | Sebtu  | Sabtu         |
| 7      | Akad   | Minggu        |

### Pasaran

Selain 7 hari, masyarakat Jawa juga membagi hari menjadi 5 (*Pasaran*):

| Pasaran | Neptu |
|---------|-------|
| Legi    | 5     |
| Pahing  | 9     |
| Pon     | 7     |
| Wage    | 4     |
| Kliwon  | 8     |

> **Neptu** adalah bobot angka dari Pasaran. Penggunaannya umum dalam adat dan penetapan acara tradisional.

### Bulan (*Sasi*)

Kalender Jawa terdiri dari 12 bulan (*sasi*):

| Urutan | Sasi          | Alias         | Jumlah Hari |
|--------|---------------|---------------|-------------|
| 1      | Mukarom       | Suro          | 30          |
| 2      | Sapar         | -             | 29          |
| 3      | Robi'ulawal   | Mulud         | 30          |
| 4      | Robi'ulakir   | Bakda Mulud   | 29          |
| 5      | Jumadilawal   | -             | 30          |
| 6      | Jumadilakir   | -             | 29          |
| 7      | Rojab         | Rejeb         | 30          |
| 8      | Sakban        | Ruwah, Arwah  | 29          |
| 9      | Romadon       | Pasa, Ramelan | 30          |
| 10     | Sawal         | -             | 29          |
| 11     | Dulkodah      | Séla          | 30          |
| 12     | Dulkijah      | Besar         | 29/30*      |

> **\*** Lihat tabel Tahun Jawa.

### Tahun Jawa

Dalam Kalender Jawa, satu *windu* (8 tahun) adalah siklus terbesar. Nama tahun dalam satu *windu*:

| Urutan | Tahun Jawa | Hari/Tahun |
|--------|------------|------------|
| 1      | Alip       | 354        |
| 2      | Ehe        | 355        |
| 3      | Jimawal    | 354        |
| 4      | Je         | 354        |
| 5      | Dal        | 355        |
| 6      | Be         | 354        |
| 7      | Wawu       | 354        |
| 8      | Jimakir    | 355        |

> Tahun dengan nama sama (misalnya, *Tahun Be*) memiliki awal tahun yang sama (misalnya, *Rebo Kliwon*).

## Rumus Matematis

Kalender Jawa memiliki keteraturan luar biasa, memungkinkan perhitungan pola-pola untuk awal bulan, tahun dan didasarkan pada rumus matematis. Kalender ini dilestarikan dari generasi ke generasi melalui rumus-rumus matematis. Ironisnya, tidak banyak generasi baru yang memahami atau menyadari ilmu ini.

### Rumus Hafalan Awal Bulan Kalender Jawa Abadi

| SASI/TAHUN IN SEWINDU          | 1. ALIP     | 2. EHE      | 3. JIMAWAL   | 4. JE       | 5. DAL     | 6. BE       | 7. WAWU     | 8. JIMAKIR   |
|---------------|-------------|-------------|-------------|-------------|------------|------------|------------|-------------|
| **1. Mukarom**      | Rom Ji Ji   | Rom Mo Mo   | Rom Lu Mo   | Rom Tu Pat  | Rom Pat Lu  | Rom Ro Lu   | Rom Nem Ro  | Rom Lu Ji   |
| **2. Sapar**        | Par Lu Ji   | Par Tu Mo   | Par Mo Mo   | Par Ro Pat  | Par Nem Lu  | Par Pat Lu  | Par Ji Ro   | Par Mo Ji   |
| **3. Robi'ulawal**  | Rowal Pat Mo| Rowal Ji Pat| Rowal Nem Pat| Rowal Lu Lu | Rowal Tu Ro | Rowal Mo Ro | Rowal Ro Ji | Rowal Nem Mo|
| **4. Robi'ulakir**  | Rokir Nem Mo| Rokir Lu Pat| Rokir Ji Pat| Rokir Mo Lu | Rokir Ro Ro | Rokir Tu Ro | Rokir Pat Ji| Rokir Ji Mo |
| **5. Jumadilawal**  | Juwal Tu Pat| Juwal Pat Lu| Juwal Ro Lu | Juwal Nem Ro| Juwal Lu Ji | Juwal Ji Ji | Juwal Mo Mo | Juwal Ro Pat|
| **6. Jumadilakir**  | Jukir Ro Pat| Jukir Nem Lu| Jukir Pat Lu| Jukir Ji Ro | Jukir Mo Ji | Jukir Lu Ji | Jukir Tu Mo | Jukir Pat Pat|
| **7. Rojab**        | Jab Lu Lu   | Jab Tu Ro   | Jab Mo Ro   | Jab Ro Ji   | Jab Nem Mo  | Jab Pat Mo  | Jab Ji Pat  | Jab Mo Lu   |
| **8. Sakban**       | Ban Mo Lu   | Ban Ro Ro   | Ban Tu Ro   | Ban Pat Ji  | Ban Ji Mo   | Ban Nem Mo  | Ban Lu Pat  | Ban Tu Lu   |
| **9. Romadon**      | Don Nem Ro  | Don Lu Ji   | Don Ji Ji   | Don Mo Mo   | Don Ro Pat  | Don Tu Pat  | Don Pat Lu  | Don Ji Ro   |
| **10. Sawal**       | Wal Ji Ro   | Wal Mo Ji   | Wal Lu Ji   | Wal Tu Mo   | Wal Pat Pat | Wal Ro Pat  | Wal Nem Lu  | Wal Lu Ro   |
| **11. Dulkodah**    | Dah Ro Ji   | Dah Nem Mo  | Dah Pat Mo  | Dah Ji Pat  | Dah Mo Lu   | Dah Lu Ji   | Dah Tu Ro   | Dah Pat Ji  |
| **12. Dulkijah**    | Jah Pat Ji  | Jah Ji Mo   | Jah Nem Mo  | Jah Lu Pat  | Jah Tu Lu   | Jah Mo Lu   | Jah Ro Ro   | Jah Nem Ji  |

[(*sumber gambar*)](https://www.caknun.com/2019/kalender-jowo-digowo-kalender-arab-digarap-kalender-barat-diruwat)

Contoh untuk menghitung awal bulan *1 Suro (Mukarom) 1953 J* (1 September 2019 M):

1. Tahun 1953 adalah *Tahun Wawu, Kurup Asapon (Alip Selasa Pon)*.
2. Rumus awal bulan *Mukarom* pada *Tahun Wawu*: **"Rom Nem Ro"** (*Mukarom Enem Loro*).  
   - 6 = hari, 2 = pasaran (dihitung dari awal Kurup: Asapon).
3. Hari ke-6 dihitung dari Selasa: Akad (Minggu).
4. Pasaran ke-2 dihitung dari Pon: Wage.
5. Hasil: **1 Suro (Mukarom) 1953 J** bertepatan dengan **Minggu Wage**.

## Referensi

1. Yudi Rohmat, [*Kalender Jowo Digowo Kalender Arab Diruwat*](https://www.caknun.com/2019/kalender-jowo-digowo-kalender-arab-digarap-kalender-barat-diruwat), caknun.com, 2019.
