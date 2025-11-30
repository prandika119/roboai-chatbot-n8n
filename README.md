# RoboAI Chatbot (n8n + Supabase + Next.js)

Ringkasan: sistem chatbot ini dirancang untuk membantu manajer hotel memantau, menganalisis, dan merespon ulasan atau keluhan tamu secara otomatis. Sistem menggunakan n8n sebagai orkestrator workflow, Supabase sebagai database, Next.js untuk tampilan halaman login dan dashboard ringan, integrasi Telegram untuk notifikasi dan interaksi, Robota API (dashboard manager hotel) sebagai integrasi sistem hotel, serta model LLM (Gemini dan/atau Ollama) untuk analisis bahasa alami dan ringkasan.

Daftar singkat teknologi:
- n8n (workflow automation)
- Supabase (Postgres, Auth, Realtime)
- Next.js (frontend untuk login dan halaman manager)
- Telegram Bot API (notifikasi dan interaksi)
- Robota API (dashboard manager hotel — integrasi eksternal)
- Gemini / Ollama (LLM untuk analisis, klasifikasi, ringkasan)

Use cases utama
1. Tanya Jawab Ringkasan Review
   - Aktor: Manajer Hotel
   - Deskripsi: Manajer dapat meminta ringkasan ulasan/keluhan mingguan. Chatbot akan mengumpulkan semua keluhan dan ulasan selama satu minggu, melakukan pemrosesan (filter, klasifikasi, ekstraksi topik), lalu menyajikan laporan ringkas yang mudah dibaca.

2. Terima Notifikasi Keluhan Penting
   - Aktor: Manajer Hotel
   - Deskripsi: Sistem akan mendeteksi keluhan yang bersifat kritis (mis. gangguan keselamatan, air bocor, masalah kebersihan berat) dan mengirim notifikasi instan ke manajer via Telegram atau endpoint notifikasi Robota.

3. Laporan Permasalahan Hotel (Actionable Reports)
   - Aktor: Manajer Hotel
   - Deskripsi: Manajer dapat meminta laporan lebih detail berdasarkan analisis data keluhan, termasuk metrik, tren, rekomendasi tindakan, dan prioritas. Laporan ini bersifat actionable untuk pengambilan keputusan (perbaikan fasilitas, pelatihan staf, dsb).


Contributing
- Buka issue jika ada fitur/bug.
- Ikuti konvensi commit, jalankan lint & unit tests jika ada.
- Sertakan migration SQL saat menambah tabel/kolom.


Kontak
- Repo: https://github.com/prandika119/roboai-chatbot-n8n
