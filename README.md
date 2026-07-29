# EME (Emergency Memo Enumerator)

**EME** adalah aplikasi manajemen penomoran surat (memo) berbasis web yang dirancang untuk efisiensi administrasi. Aplikasi ini mengotomatisasi pembuatan nomor surat, pengelolaan data, dan penyajian informasi dengan antarmuka yang bersih dan profesional bergaya *SAP Enterprise*.

## Fitur Utama

*   **Smart Auto-Numbering**: Sistem penomoran otomatis yang cerdas. Menghitung urutan berdasarkan data terakhir di database, memastikan nomor selalu akurat (Contoh: 385/PPBJE/D2350/VII/2026 -> 386/...).
*   **SAP-Style Interface**: Desain antarmuka *enterprise* yang bersih, *data-dense*, dan mudah dinavigasi.
*   **Interactive Table**: 
    *   Sortir data secara *real-time* (Ascending/Descending) hanya dengan klik header.
    *   *Fixed Table Layout* untuk menjaga kerapihan tampilan.
*   **CRUD Operations**: Kemampuan untuk menambah, mengedit, dan menghapus data dengan mudah.
*   **Data Management**: 
    *   Pagination (Paging) dengan fitur *Jump-to-Page* yang cepat.
    *   Input yang diperluas untuk field "Uraian Isi" dan "Keterangan".
*   **Lightweight**: Berjalan dengan Vanilla JavaScript, HTML5, dan CSS3 tanpa ketergantungan framework berat.

## Persyaratan (Prerequisites)

Karena aplikasi ini menggunakan `fetch` untuk memuat data JSON lokal, browser tidak mengizinkan akses langsung dari protokol `file:///`.

1.  **Web Server Lokal**: Wajib menjalankan server lokal agar aplikasi berjalan.
    *   **VS Code**: Gunakan ekstensi "Live Server".
    *   **Python**: Jalankan `python -m http.server 8000` di direktori proyek.
    *   **Node.js**: Gunakan `http-server` atau sejenisnya.

## Struktur File

```text
├── index.html            # Aplikasi utama
├── rekap_surat_data.json # Database file (format JSON)
└── README.md             # Dokumentasi ini
