# RSI Signal App v8 — XAUUSD & NASDAQ

Aplikasi web mandiri (tanpa TradingView). RSI dihitung langsung di browser (RSI 8, Close, metode Wilder).

## Sinyal
- BUY saat RSI menyentuh 30 ke bawah (BUY+ di 20, BUY++ di 15)
- SELL saat RSI menyentuh 70 ke atas (SELL+ di 80, SELL++ di 85)
- Sinyal muncul sekali saat RSI baru masuk zona. Entry/SL/TP (ATR 14 × 1,5, TP 2R) untuk level 30/70.
- Mode: saat candle tutup (default, tidak repaint) atau live.
- Notifikasi suara, getar, dan browser saat sinyal baru muncul (aplikasi harus terbuka).

## Sumber data (v5: otomatis, dengan cadangan)
- Emas: Binance Futures XAUUSDT, lalu Binance PAXG (token emas), lalu Yahoo Finance (GC=F).
- NASDAQ: Twelve Data (jika API key diisi), lalu Yahoo Finance (NQ=F, futures Nasdaq 100).
- Sumber yang dipakai ditampilkan di bawah chart. Harga bisa sedikit berbeda dari broker/TradingView.

## Deploy GitHub Pages
Upload `index.html` dan `.nojekyll` ke repository, lalu Settings > Pages > Deploy from a branch > main / root.
File `RSI_Signal_TradingView.pine` bersifat opsional (khusus TradingView).

Alat bantu analisis, bukan rekomendasi transaksi.

## v6 — Data dari MT5 sendiri
Aplikasi RSI membaca candle broker lewat aplikasi sinyal Anda (Vercel): `GET /api/candles`.
Wajib: upload `app.py` (v19.3) ke repository aplikasi sinyal, EA SinyalMT5 berjalan, dan sebaiknya Upstash Redis aktif di Vercel.

## v7
- Timeframe M15/M30/H1 otomatis disusun dari data M5 MT5 bila candle TF itu belum dikirim EA.
- Tampilan lama dibersihkan saat data gagal dimuat (tidak lagi menampilkan angka TF sebelumnya).

## v8
- Pilihan pair (XAUUSD/NASDAQ) dan timeframe menempel di bagian atas layar saat halaman digulir.
- Pengaturan disembunyikan; buka lewat tombol ⚙.
- Riwayat sinyal dibuat ringkas dan bisa digeser (scroll) di dalam kotaknya.
