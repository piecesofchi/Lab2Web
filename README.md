# Lab2Web - Praktikum 2: CSS Dasar

---

## Langkah Praktikum

### 1. Membuat File HTML Dasar
Saya membuat file `lab2_css_dasar.html` berisi struktur HTML dasar untuk latihan CSS.  
Hasil awal (sebelum CSS eksternal):  
<img width="960" height="600" alt="5" src="https://github.com/user-attachments/assets/154b2a50-5c1c-441a-a259-5e7f972de4b6" />

---

### 2. Menambahkan Internal CSS
Saya menambahkan internal CSS di dalam tag `<head>` menggunakan `<style>`.  
Internal CSS ini mengatur font, warna judul, dan border pada header.  
<img width="960" height="600" alt="6" src="https://github.com/user-attachments/assets/26330840-c30f-4b87-8361-75bccc8c3e83" />


---

### 3. Menambahkan Inline CSS
Saya menambahkan inline CSS langsung di dalam tag `<p>` menggunakan atribut `style`.  
Contoh:  
```html
<p style="color: red; text-align: center;">Ini paragraf dengan inline CSS</p>

---

4. Membuat File CSS Eksternal

Saya membuat file style_eksternal.css lalu menambahkan kode CSS untuk:

Mengatur background menu navigasi (nav).

Memberi warna pada bagian intro (#intro).

Memberi style pada tombol dengan class .button dan .btn-primary.


File CSS eksternal dihubungkan menggunakan tag <link> di bagian <head>.



---

5. Menguji CSS Selector

Saya mencoba perbedaan selector:

h1 { ... } berlaku untuk semua elemen <h1>.

#intro h1 { ... } hanya berlaku untuk elemen <h1> di dalam id="intro".
Hasil: teks judul dalam intro berbeda warna dengan judul lainnya.



---

6. Menguji Prioritas CSS (Cascade)

Saya mencoba kasus di mana satu elemen memiliki aturan dari eksternal, internal, dan inline CSS sekaligus.
Hasilnya:

Inline CSS menang terhadap internal dan eksternal.

Internal CSS menang terhadap eksternal.




---

Jawaban Pertanyaan Teori

2. Apa perbedaan h1 {…} dengan #intro h1 {…}?

h1 {…} berlaku untuk semua elemen <h1> di halaman.

#intro h1 {…} hanya berlaku untuk <h1> yang ada di dalam elemen dengan id="intro".


3. Jika ada internal, eksternal, dan inline CSS pada elemen yang sama, mana yang ditampilkan?

Prioritas: Eksternal < Internal < Inline.

Jadi kalau semua dipakai sekaligus, yang menang adalah Inline CSS.


4. Jika sebuah elemen memiliki ID dan Class sekaligus, mana yang dipakai?

Selector ID (#id) lebih kuat dibanding selector Class (.class).

Jadi kalau ada konflik, CSS pada ID yang dipakai.
Contoh:


#paragraf-1 { color: green; }
.text-paragraf { color: blue; }

<p id="paragraf-1" class="text-paragraf">Contoh teks</p>

 Teks akan berwarna hijau (karena ID lebih spesifik).


---

Kesimpulan

Pada praktikum ini saya berhasil:

Membuat file HTML dengan CSS internal, inline, dan eksternal.

Memahami penggunaan selector (elemen, class, dan id).

Memahami prioritas penerapan CSS (cascade).

Membuat laporan praktikum berupa README.md dengan dokumentasi screenshot.
