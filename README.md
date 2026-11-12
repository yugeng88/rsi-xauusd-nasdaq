# RSI Learning Dashboard — XAUUSD & NASDAQ

Dashboard statis untuk GitHub Pages. Hanya menampilkan chart publik TradingView dengan indikator RSI periode 8 dan sumber harga yang jelas.

## Pengaturan
- Instrumen XAUUSD: `OANDA:XAUUSD` (emas spot)
- Instrumen NASDAQ: `CME_MINI:NQ1!` (E-mini Nasdaq-100 futures)
- Timeframe: M5, M15, M30, H1
- Indikator: Relative Strength Index (RSI)
- Periode: 8
- Sumber harga indikator: Close
- Level referensi: 15, 20, 30, 50, 70, 80, 85

## Isi paket
- `index.html` — aplikasi utama
- `README.md` — dokumentasi
- `GITHUB_PAGES_ID.md` — panduan upload GitHub Pages
- `.nojekyll` — file konfigurasi GitHub Pages

## Upload / update ke repository GitHub
Repository yang digunakan: `yugeng88/rsi-xauusd-nasdaq`.

1. Ekstrak ZIP.
2. Buka repository GitHub.
3. Pilih **Add file → Upload files**.
4. Upload dan timpa `index.html`, `README.md`, `GITHUB_PAGES_ID.md`, dan `.nojekyll`.
5. Tekan **Commit changes**.
6. Buka **Settings → Pages**. Pastikan source `Deploy from a branch`, branch `main`, folder `/(root)`.
7. Tunggu deployment, lalu buka `https://yugeng88.github.io/rsi-xauusd-nasdaq/`.

## Tentang data
Dashboard ini memakai widget chart publik TradingView. Ia tidak mengambil atau menyalin sinyal transaksi, entry, SL, TP, atau data privat dari aplikasi `sinyal-xauusd.vercel.app`. Chart memerlukan koneksi internet dan dapat gagal dimuat jika layanan TradingView diblokir oleh jaringan/peramban. Harga dapat berbeda dari feed broker.

RSI adalah indikator edukatif, bukan prediksi pasti atau rekomendasi transaksi. Level 15/85 adalah level RSI, bukan harga stop-loss.
