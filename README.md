**TODO**

- logo menyebabkan **Layout Shifting** pada bagian index.hbs page
  solusi : buat DIV nya punya width dan height yang tetap
- ambil gambar UMKM dari google drive untuk dipasang di **caresoul** dan page **belanja.hbs**

  ```html
  <image src="link download url from g.drive">
  ```
- ADMIN umkm: form input data UMK
- pasang di **server.js** sebagai 404 redirect

  ```javascript
  fastify.setNotFoundHandler(handler(request, reply))
  ```
- **riwayat.hbs,** ubah status (ada ket. RT/RW dan proses kelurahan) berkas menjadi sudah atau belum
- **pesan.hbs**, pesan masuk dari admin

  ```html
  <button type="button" class="btn btn-primary position-relative">
    Profile
    <span class="position-absolute top-0 start-100 translate-middle p-2 bg-danger border border-light rounded-circle">
      <span class="visually-hidden">New alerts</span>
    </span>
  </button>
  ```
- **pengaduan.hbs,** warga mengirim pesan ke admin
- **belanja.hbs,** ambil data pemilik usaha dan gambar produknya
  - atur di _appscript_ kembalikan `getDownloadUrl()`
- **belanja.hbs,** buatkan filter kategori

  ```html
  <div class="btn-group" role="group" aria-label="Basic radio toggle button group">
    <input type="radio" class="btn-check" name="btnradio" id="btnradio1" autocomplete="off" checked>
    <label class="btn btn-outline-primary" for="btnradio1">Radio 1</label>
  
    <input type="radio" class="btn-check" name="btnradio" id="btnradio2" autocomplete="off">
    <label class="btn btn-outline-primary" for="btnradio2">Radio 2</label>
  
    <input type="radio" class="btn-check" name="btnradio" id="btnradio3" autocomplete="off">
    <label class="btn btn-outline-primary" for="btnradio3">Radio 3</label>
  </div>
  ```
- TTE - RT/RW (QR-Code) pakai <https://davidshimjs.github.io/qrcodejs/>
- pengaturan =&gt; ganti password
