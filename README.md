# RSI Signal App v4 — XAUUSD & NASDAQ

Aplikasi web mandiri (tanpa TradingView). RSI dihitung langsung di browser (RSI 8, Close, metode Wilder).

## Sinyal
- BUY saat RSI menyentuh 30 ke bawah (BUY+ di 20, BUY++ di 15)
- SELL saat RSI menyentuh 70 ke atas (SELL+ di 80, SELL++ di 85)
- Sinyal muncul sekali saat RSI baru masuk zona. Entry/SL/TP (ATR 14 × 1,5, TP 2R) untuk level 30/70.
- Mode: saat candle tutup (default, tidak repaint) atau live.
- Notifikasi suara, getar, dan browser saat sinyal baru muncul (aplikasi harus terbuka).

## Sumber data
- Binance Futures (default, tanpa API key): XAUUSDT (emas). NASDAQ belum tersedia di sumber ini.
- Twelve Data (API key gratis di twelvedata.com): XAU/USD dan NDX. Jika NDX tidak tersedia di paket Anda, ganti simbol di Pengaturan.

## Deploy GitHub Pages
Upload `index.html` dan `.nojekyll` ke repository, lalu Settings > Pages > Deploy from a branch > main / root.
File `RSI_Signal_TradingView.pine` bersifat opsional (khusus TradingView).

Alat bantu analisis, bukan rekomendasi transaksi.
