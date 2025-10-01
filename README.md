1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS
    dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan
    penjelasannya!
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada
    elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan
    penjelasan dan contohnya!
4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut
    terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
    Berikan penjelasan dan contohnya! ( <p id="paragraf-1" class="text-paragraf"> )# Lab2Web

                                   Jawaban
1. (https://1drv.ms/i/c/45165ae86f98468c/EY3X4hSEf9xDtT6MJDRPGWcBHfmsetVLRoYWn8EY1aL4IQ?e=e9xQDL)

2. h1 { ... }
Selector ini langsung menargetkan semua elemen <h1> di halaman web.
Jadi semua <h1> akan mendapatkan style yang sama.

#intro h1 { ... }
Selector ini lebih spesifik:
Artinya hanya <h1> yang berada di dalam elemen dengan id="intro" yang akan kena style.

3. Ketika browser membaca CSS, ada aturan yang namanya CSS Cascade (urutan prioritas).
Jadi, jika ada banyak deklarasi pada elemen yang sama, browser akan memilih deklarasi dengan tingkat prioritas tertinggi.

Eksternal CSS
Disimpan di file terpisah (style.css) lalu dipanggil dengan <link>.
Posisinya paling lemah, karena berlaku global untuk seluruh halaman.

Internal CSS
Didefinisikan di dalam file HTML, di tag <style> pada <head>.
Prioritasnya lebih tinggi daripada eksternal karena berada langsung di dokumen HTML.

Inline CSS
Ditulis langsung di atribut style="" pada elemen HTML.
Inline punya prioritas lebih tinggi dibanding internal & eksternal karena menempel langsung di elemen.

!important
Jika ada properti yang diberi !important, maka aturan ini akan menimpa semua prioritas lain.

4. Urutan kekuatan selector CSS
- Element selector (misalnya p, h1) → paling lemah.
- Class selector (.text-paragraf, .container)
- ID selector (#paragraf-1)
- Inline CSS (style="...") → lebih kuat dari semua selector.
- !important → paling tinggi, menimpa semuanya.

Penjelasan
Class bisa dipakai berkali-kali pada banyak elemen → sifatnya umum.
ID hanya boleh dipakai unik sekali dalam satu halaman → sifatnya spesifik.
Karena lebih spesifik, maka deklarasi ID menang dibandingkan deklarasi Class pada elemen yang sama.

Jadi Deklarasi CSS dengan selector #id akan ditampilkan di browser, karena ID memiliki prioritas lebih tinggi daripada Class.
