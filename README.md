# Deploy Aplikasi Flask

Project Flask minimalis yang gampang banget dipakai buat bikin aplikasi web simpel dan ringan. Semua kodenya cuma di satu file (`app.py`), plus ada template HTML dan file statis dasar biar gampang dikembangin.

## Fitur

* Aplikasi Flask cuma satu file (`app.py`), jadi gak ribet dan cepet paham.
* Struktur template HTML sederhana, ada sedikit styling dan JavaScript.
* Setup gampang tanpa hal-hal yang nggak perlu.
* Bisa kamu modifikasi dengan cepat buat bikin aplikasi web sendiri.

## Cara Instalasi dan Setup di AWS
1. Fork repo flask-minimal paknux ke akun GitHub kamu.

2. Buat instance Ubuntu di AWS EC2:

   * Pilih Amazon Machine Image (AMI) Ubuntu terbaru.

   * Saat setup Security Group, tambahkan aturan inbound rule untuk port 5000 dengan sumber 0.0.0.0/0 supaya aplikasi bisa diakses dari mana saja.

   * Jangan lupa juga tambahkan port 22 untuk SSH akses.

3. Connect ke instance Ubuntu
   
## Persiapan

Jalankan perintah ini dulu buat update dan install Python beserta toolsnya:

```bash
sudo apt update
sudo apt install python3 python3-venv python3-pip -y
```

## Cara Instalasi

1. Clone project ini ke komputer kamu:

   ```bash
   git clone https://github.com/yourusername/flask-minimal.git
   cd flask-minimal
   ```

2. Buat virtual environment (biar bersih dan rapi):

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Install semua package yang dibutuhkan:

   ```bash
   pip install -r requirements.txt
   ```

4. Jalankan aplikasinya:

   ```bash
   python app.py
   ```

Buka browser kamu dan akses [http://localhost:5000](http://localhost:5000) buat lihat aplikasinya.
