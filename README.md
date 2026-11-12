# RSI Dashboard — XAUUSD & NASDAQ

## Konfigurasi
- NASDAQ: `FX:NAS100` (US 100 Index · FX)
- XAUUSD: `OANDA:XAUUSD`
- RSI: periode 8, source Close
- Level: 15, 20, 30, 50, 70, 80, 85
- Timeframe dashboard: M5, M15, M30, H1
- Sinyal Pine Script: BUY (RSI <= 30), SELL (RSI >= 70), SIDEWAY (RSI di antara 30 dan 70)

## Isi ZIP
- `index.html`: dashboard responsif untuk iPhone dan desktop dengan chart TradingView.
- `RSI_Signal_TradingView.pine`: indikator Pine Script dengan label status, marker perubahan sinyal, dan alertcondition.
- `.nojekyll`: file pendukung GitHub Pages.

## Cara menggunakan
1. Ekstrak ZIP.
2. Upload semua file ke repository GitHub.
3. Buka Settings > Pages.
4. Pada Build and deployment, pilih Deploy from a branch, branch `main`, folder `/ (root)`, lalu Save.
5. Buka alamat GitHub Pages yang diberikan GitHub.
6. Untuk mengaktifkan sinyal otomatis, buka TradingView > Pine Editor.
7. Buka file `RSI_Signal_TradingView.pine`, salin seluruh isinya ke Pine Editor, lalu pilih Save dan Add to chart.
8. Pilih simbol `FX:NAS100` atau `OANDA:XAUUSD` dan timeframe M5/M15/M30/H1.
9. Buat Alert pada indikator ini. Pilih kondisi RSI BUY, RSI SELL, atau RSI SIDEWAY sesuai kebutuhan.

## Catatan teknis penting
GitHub Pages adalah hosting statis. TradingView Advanced Chart Embed tidak menyediakan API browser untuk membaca nilai RSI dari widget atau menerima alert akun secara langsung. Karena itu, Pine Script menjalankan perhitungan dan alert di TradingView. Marker sinyal terlihat pada chart dan riwayat historisnya mengikuti bar yang dimuat TradingView; halaman GitHub Pages tidak dapat menampilkan riwayat alert akun TradingView secara otomatis tanpa endpoint/backend tambahan.

Widget RSI bawaan TradingView ditampilkan sebagai referensi. Untuk memastikan seluruh level 15, 20, 30, 50, 70, 80, 85 dan sinyal BUY/SELL/SIDEWAY, pasang Pine Script yang disertakan.

## Disclaimer
Indikator bersifat alat bantu analisis, bukan rekomendasi transaksi atau jaminan profit. Periksa data, sesi, spread, dan karakteristik simbol broker sebelum mengambil keputusan.
