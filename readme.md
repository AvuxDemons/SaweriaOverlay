# About

![Osakana](https://media.discordapp.net/attachments/972016247795515454/1126388003938508860/osakana.png)

Tingkatkan pengalaman donasi Anda dengan Saweria Custom Overlay Donation Alert! Ubah tampilan dan pesan donasi secara kreatif, sampaikan apresiasi secara real-time, dan buat pengalaman donasi yang tak terlupakan. Coba sekarang dan berikan sentuhan khusus pada setiap donasi yang masuk!

# Documentation
* [Setup](#installation)
    - [Saweria](#saweria)
    - [Tema](#tema)
    - [OBS](#setup-obs--wajib)
* [Configuration](#configuration)
    - [Background Images](#background-images)
    - [Custom Mascot](#custom-mascot)
    - [Custom Text](#custom-text)
    - [Custom Color](#custom-color)
* [List Tema](#theme-preview)
* [Miscellaneous](#miscellaneous)
    - [Contributing](#contributing)
    - [Theme Requests](#theme-requests)
    - [Feature Requests](#contributions)
    - [Commission](#commission)

# Installation

Berikut merupakan cara menggunakan Custom Overlay Saweria
#### Video : [Tonton Video Tutorial Di Youtube](https://youtu.be/I2QZUQXBTsE)
<br>

## Setup Custom Overlay Saweria
### [+] Saweria
1. Cara akses Custom Overlay Saweria
    ![anya_peek](https://saweria.co/custom-overlay-access.png)
    Buka halaman [pengaturan overlay saweria](https://saweria.co/overlays) dan klik custom pada ujung kanan atas dialog Tampilan seperti gambar diatas
    
### [+] Tema
2. Pilih tema Custom Saweria Overlay pada [Theme Preview](#theme-preview)
3. Klik pada nama tema yang akan digunakan 
    ![Select](https://media.discordapp.net/attachments/972016247795515454/1126400261649338408/image.png)
4. Klik File `index.html` Dan Copy / Salin seluruhnya atau mulai dari `<div> sampai </div>`
    ![copy html](https://cdn.discordapp.com/attachments/972016247795515454/1126400984889954384/image.png)
    Kemudian Paste / Tempel pada kolom `HTML` di halaman pengaturan overlay saweria ( Jika kolom HTML tidak kosong , Harap kosongi terlebih dahulu / Replace saja dengan yang telah anda Copy / Salin )
5. Klik File `style.css` Copy / Salin seluruhnya kemudian Paste / Tempel pada kolom `CSS` di halaman pengaturan overlay saweria
6. Pada kolom `Durasi Notifikasi (ms)` isikan minimal `10000` ( 10 detik)
7. Klik `Simpan Tampilan` & Custom Saweria Overlay anda siap digunakan 

[-] Tambahan ( Animasi )

1. [Buka Folder Animation](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/animation)
2. Pilih Tipe Animasi
    - Container ( Keseluruhan Overlay )
    - Text ( Hanya Text nya Saja )
3. Klik File Model Animasi Yang Di Inginkan
4. Copy / Salin Seluruhnya Kemudian Paste / Tempel pada kolom `CSS` di halaman pengaturan overlay saweria ( Paste / Tempel dibawah CSS tema [ Jangan di Replace ] )

### [+] Setup OBS / SL OBS ( WAJIB )

**MINIMUM** Source Properties [ Width - `1000` ]  & [ Height - `600` ] <br>
Setelah merubah tampilan overlay , single click pada browser source Overlay Saweria di OBS dan tekan `Refresh` atau double click dan tekan `Refresh cache of current page`.

Jika tidak tampil, pastikan OBS telah terupdate ke versi terbaru (v28).

<br>

# Configuration

## Background Images
Anda dapat mengubah background Overlay anda
1. Cari bagian berikut pada file `index.html`
    ```
    <div class="container">
        <img alt="Background Image" src="https://domain.com/image.jpg" class="background-img">

        <!-- code -->
    </div>
    ```
2. Silahkan Replace url pada bagian `src=" Taruh URL Gambar Background Anda Disini "`

## Custom Mascot

1. Cari bagian berikut pada file `index.html`
    ```
    <div class="container">
        <!-- code  -->

            <div class="mascot">
                <img src="https://domain.com/image.jpg">
            </div>
        
        <!-- code -->
    </div>
    ```
2. Silahkan Replace url pada bagian `src=" Taruh URL Gambar Mascot Anda Disini "`

## Custom Text

1. Cari bagian berikut pada file `index.html`
    ```
    <div class="container">
        <!-- code -->

            <div class="text">
                <p>
                    <span class="amount">{amount}</span>
                    Dari 
                    <span class="donator">{donator}</span>
                </p>
                <p>
                    <span class="message">
                        {message}
                    </span>
                </p>

        <!-- code -->
    </div>
    ```
2. Anda dapat merubah teks yg tidak berada di dalam `<span> - </span>` sesuai dengan keinginan anda .

Note* berikut beberapa token yang disediakan oleh Saweria untuk teks yang berada di dalam `<span> - </span>`
- `{media}`
- `{message}`
- `{donator}`
- `{amount}`

## Custom Color

1. Cari bagian berikut pada file `style.css`
    ```
    :root {
        --amount: rgb(223, 168, 102);
        --donator: rgb(223, 168, 102);
        --text: #ffffff;
    }
    ```
2. Ubah dengan warna yang sesuai dengan keinginan anda. Gunakan [Color Conversion](https://imagecolorpicker.com/color-code/ffffff) jika anda tidak mengetahui code warna. Anda dapat menggunakan semua konversi yang ada pada web tersebut. ( disarankan menggunakan HEX Color )
<br>

# Theme Preview

### [Anya Peeking | GIF](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/template/anya_peek)

![anya_peek](https://media.discordapp.net/attachments/972016247795515454/1126384061687025714/anyapeek.png)

### [Anya Waku | GIF](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/template/anya_peek)

![anya_waku](https://cdn.discordapp.com/attachments/972016247795515454/1126384901869031504/anyawaku.png)

### [Azusa](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/template/azusa)

![azusa](https://media.discordapp.net/attachments/972016247795515454/1126388002743132240/azusa.png)

### [Emilia](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/template/emilia)

![emilia](https://media.discordapp.net/attachments/972016247795515454/1126388003066085446/emilia.png)

### [Gojo | GIF](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/template/gojo)

![gojo](https://media.discordapp.net/attachments/972016247795515454/1126388003506507806/gojo.png)

### [JDM](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/template/jdm)

![jdm](https://media.discordapp.net/attachments/972016247795515454/1126388005695934535/jdm.png)

### [Mio](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/template/mio)

![mio](https://media.discordapp.net/attachments/972016247795515454/1126388004802527242/mio.png)

### [Mugi](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/template/mugi)

![mugi](https://media.discordapp.net/attachments/972016247795515454/1126388004534100018/mugi.png)

### [Nezuko | GIF](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/template/nezuko)

![nezuko](https://media.discordapp.net/attachments/972016247795515454/1126388004248899605/nezuko.png)

### [Osakana | GIF](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/template/osakana)

![osakana](https://media.discordapp.net/attachments/972016247795515454/1126388003938508860/osakana.png)

### [Rem](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/template/rem)

![rem](https://media.discordapp.net/attachments/972016247795515454/1126388125967601726/rem.png)

### [Ritsu](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/template/ritsu)

![ritsu](https://media.discordapp.net/attachments/972016247795515454/1126388125585907743/ritsu.png)

### [Sakura](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/template/sakura)

![sakura](https://media.discordapp.net/attachments/972016247795515454/1126388125275541584/sakura.png)

### [Yui](https://github.com/AvuxDemons/SaweriaOverlay/tree/master/template/yui)

![yui](https://cdn.discordapp.com/attachments/972016247795515454/1157709372089176175/image-removebg-preview.png)

# Miscellaneous

## Contributing

Repository ini dibuka untuk umum , Anda dapat berkontribusi juga pada Repository ini.

## Theme Requests

Tidak menemukan overlay dengan tema keinginan anda ? Silahkan untuk [submit theme request](https://github.com/AvuxDemons/SaweriaOverlay/issues).

## Feature Requests

Anda memiliki saran fitur untuk Repository ini ? Silahkan untuk [submit feature request](https://github.com/AvuxDemons/SaweriaOverlay/issues).

## Commission

Ingin memiliki tema pribadi yang sesuai dengan keinginan anda ? [submit commission request](https://instagram.com/d.avux).
