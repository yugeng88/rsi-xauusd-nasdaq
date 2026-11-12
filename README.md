# RSI Signal Dashboard — XAUUSD & NASDAQ

Aplikasi web statis untuk GitHub Pages. Hanya memuat dua instrumen:
- XAUUSD (menggunakan `GC=F`, gold futures, sebagai proxy)
- NASDAQ (menggunakan `NQ=F`, Nasdaq-100 futures, sebagai proxy)

## Strategi RSI
- Periode RSI: **8**
- Apply to: **Close**
- Full Sell: **80**
- R Sell: **70**
- Sideway: **50**
- R Buy: **30**
- Full Buy: **20**
- Level ekstrem / referensi SL RSI: **85** dan **15**

RSI dihitung dengan smoothing Wilder. Klasifikasi: RSI >= 80 Full Sell; 70–<80 R Sell; >30–<70 Sideway; >20–30 R Buy; <=20 Full Buy.

## Menjalankan
Tidak perlu Python, API key, atau build:
1. Buka `index.html` di browser untuk uji tampilan. Pengambilan data membutuhkan koneksi internet.
2. Upload seluruh isi folder ini ke repository GitHub.
3. Aktifkan GitHub Pages (panduan ada di `GITHUB_PAGES_ID.md`).

## Catatan penting tentang data
Aplikasi meminta candle publik Yahoo Finance:
- `GC=F` untuk emas berjangka sebagai pendekatan XAUUSD.
- `NQ=F` untuk futures Nasdaq-100 sebagai pendekatan NASDAQ.

Keduanya **bukan** harga CFD broker yang persis sama. Simbol, spread, jam perdagangan, dan harga dapat berbeda. Yahoo Finance juga dapat membatasi permintaan atau mengubah endpoint. Jika gagal dimuat, coba Refresh atau gunakan sumber data broker sendiri.

## Disclaimer
Aplikasi ini hanya alat edukasi dan pembacaan indikator. Sinyal RSI bukan rekomendasi transaksi, bukan prediksi pasti, dan tidak menjamin hasil. Level 15/85 adalah level RSI, bukan harga stop-loss. Uji dan verifikasi data terlebih dahulu.
