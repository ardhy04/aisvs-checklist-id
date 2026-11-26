# Hasil pemeriksaan checklist OWASP AISVS v1.01

Pemeriksaan oleh AISVS Reviewer menggunakan GPT‑6.2 Sol dengan penalaran extra high. Pemeriksaan mencakup isi checklist dan referensi lokal. Status cakupan di bawah menunjukkan hubungan antar dokumen dan belum merupakan hasil pengujian aplikasi.

## Perbaikan terjemahan

Pada tahap awal, **59 dari 282 kontrol** diperbaiki dalam [checklist bahasa Indonesia](OWASP-AISVS-v1.01-Checklist-ID.xlsx). Seluruh ID, level, tabel, filter, dan pilihan status telah diverifikasi setelah perubahan.

| ID | Perbaikan yang diterapkan |
|---|---|
| C2.2.2 | Objek klasifikasi diperjelas menjadi konten prompt. |
| C6.2.3 | Build harus gagal jika metadata komponen AI BOM tidak lengkap. |
| C9.1.1–2 | Runtime menegakkan kuota dan batas eksekusi. |
| C10.3.1 dan C10.3.3 | Nama transport Streamable HTTP dan header Origin serta Host dipertahankan. |
| C10.4.7 | Dialog persetujuan dan opsi pembatalan ditampilkan sebelum pemasangan selesai. |
| AC.5.1 | Urutan jejak audit dikembalikan menjadi prompt → respons → commit → build → deployment. |
| AC.14.1 | Notifikasi regulator dilakukan jika ketentuan itu berlaku. |

## Pemeriksaan sumber AISVS

Seluruh **213 kontrol utama** dan **69 kontrol Lampiran C** cocok dari sisi ID dan level. Teks Inggris cocok dengan PDF dan Markdown setelah format Markdown dan pemenggalan baris diabaikan. Kontrol utama terdapat pada hlm. 14–40 dan Lampiran C pada hlm. 68–79. Lampiran A berisi glosarium dan Lampiran B mengindeks 213 kontrol utama. Hlm. 10–13 menjelaskan cakupan dan penggunaan AISVS bersama ASVS pada level yang sama. [PDF AISVS](https://github.com/OWASP/AISVS/releases/tag/v1.01) · [Sumber Markdown](https://github.com/OWASP/AISVS/tree/v1.01/1.01/en)

## Pemeriksaan AI Testing Guide v1

Reviewer memetakan 32 keluarga pengujian dalam empat kelompok. [PDF AI Testing Guide](https://owasp.org/projects/ai-testing-guide)

| Kelompok | Kontrol AISVS terkait | Cakupan yang perlu dilengkapi |
|---|---|---|
| Aplikasi, hlm. 67–135 | C2, C5, C7–C10, C11.3, C12.3 | Evaluasi bias keluaran yang lebih luas (APP-10, hlm. 122), ketergantungan berlebihan pada AI (APP-13, hlm. 132), dan keterjelasan keputusan bagi pengguna (APP-14, hlm. 135). |
| Model, hlm. 139–157 | C1.3, C3.5, C8.2, C11, C12.3 | Kriteria performa pada data baru atau di luar distribusi (MOD-06, hlm. 154). |
| Infrastruktur, hlm. 161–176 | C3, C6, C9, C10 | Kerahasiaan artefak model selama pengembangan dan pelatihan (INF-06, hlm. 176). |
| Data, hlm. 180–191 | C1.1, C1.3, C5.2.3, C7.3.3, C9.1.1, C11.2, C12.2.6 | Keterwakilan populasi dan skenario dalam dataset (DAT-03, hlm. 185) serta mekanisme persetujuan yang dapat diaudit (DAT-05, hlm. 191). |

## Pemeriksaan dua Top 10 OWASP

Setiap risiko memiliki kontrol AISVS terkait. Pemetaan ini menunjukkan titik awal verifikasi. Nomor halaman mengikuti nomor yang tercetak di PDF. [PDF Top 10 LLM 2026](https://genai.owasp.org/resource/owasp-genai-llm-top-10-2026/) · [PDF Top 10 Agentic 2026](https://genai.owasp.org/top-10-for-agentic-applications-2026/)

| Top 10 LLM | Kontrol AISVS terkait | Top 10 Agentic | Kontrol AISVS terkait |
|---|---|---|---|
| LLM01, hlm. 10–17 | C2.1, C9.3.5, C10.4.2 | ASI01, hlm. 9–11 | C2.1.3, C2.1.6, C9.2.5, C12.2.1 |
| LLM02, hlm. 18–22 | C5.2.2–4, C8.2.1, C11.2 | ASI02, hlm. 12–14 | C9.1.1, C9.2.1–2, C9.3.1–4, C9.5.1 |
| LLM03, hlm. 23–26 | C9.2, C9.3.1, C9.5 | ASI03, hlm. 15–17 | C5.1.2, C9.4.1–3, C9.5.2–7 |
| LLM04, hlm. 27–32 | C3.1, C6, AC.9 | ASI04, hlm. 18–20 | C6, C9.3.7, C10.1, AC.9 |
| LLM05, hlm. 33–37 | C1.3, C3.5, C8.2.3–5, C11.4.3 | ASI05, hlm. 21–23 | C4.1.1–2, C7.1.1, C9.3.1, AC.11.3 |
| LLM06, hlm. 38–42 | C2.1.4, C9.1, C11.2.2, C12.2.5 | ASI06, hlm. 24–26 | C8, C12.5.4 |
| LLM07, hlm. 43–45 | C7.2, C7.4.2–3, C12.3.2–3 | ASI07, hlm. 27–29 | C5.1.2, C9.4.1–2, C10.3.1, C10.3.4–5, C10.4.6 |
| LLM08, hlm. 46–49 | C7.3.2, C9.5.3–4 | ASI08, hlm. 30–32 | C9.1.1–3, C9.2.10–11, C9.6 |
| LLM09, hlm. 50–54 | C5.2.2, C8, C12.1.4 | ASI09, hlm. 33–35 | C9.2.1–4, C7.2.2–3, C7.4 |
| LLM10, hlm. 55–57 | C7.1, C7.3.3–4, C10.4.1 | ASI10, hlm. 36–38 | C9.4, C9.6.1–3, C12.4, AC.14 untuk CI/CD |

### Cakupan tambahan LLM

- **LLM02 dan LLM09.** Verifikasi penghapusan data pada data mentah, embedding, checkpoint, dan adaptor sesuai cakupan serta batas waktu yang berlaku (hlm. 20–22 dan 52–53).
- **LLM06.** Verifikasi plafon biaya per pengguna, tim, atau akun, dan apakah fungsi penting tetap tersedia saat beban tinggi (hlm. 40–41).
- **LLM07.** Verifikasi klaim penting terhadap sumber yang berwenang dan terkini sebelum digunakan untuk mengambil tindakan (hlm. 44).
- **LLM10.** Lengkapi verifikasi dengan kontrol ASVS yang sesuai, termasuk pengodean keluaran sesuai konteks dan kueri terparameterisasi (hlm. 56–57).

Sampul salinan LLM 2026 di folder masih memuat placeholder tanggal publikasi.

### Cakupan tambahan Agentic

- **ASI07.** Verifikasi autentikasi dua arah, integritas pesan, perlindungan terhadap pengiriman ulang, dan kontrak pesan antaragen di luar MCP (hlm. 28–29).
- **ASI08.** Verifikasi batas penyebaran kegagalan antarkomponen (hlm. 32).
- **ASI09.** Verifikasi jalur pelaporan pengguna dan informasi risiko sebelum pengguna memberi persetujuan (hlm. 34–35).
- **ASI10.** Verifikasi perilaku agen secara berkala dan sebelum agen diaktifkan kembali setelah karantina (hlm. 37–38).

Sebagian rujukan internal Agentic memakai nomor LLM edisi 2025. Dalam edisi 2026, Excessive Agency terpetakan ke LLM03 dan Improper Output Handling ke LLM10.
## Tindak lanjut

Ke-20 item verifikasi pelengkap telah dimasukkan ke tab **Verifikasi Tambahan** dalam [checklist bahasa Indonesia](OWASP-AISVS-v1.01-Checklist-ID.xlsx). Item PL-01 sampai PL-20 mencantumkan rujukan sumber, halaman, kontrol terkait, dan contoh bukti. Status awal setiap item adalah **Belum Diuji**.

## Verifikasi ulang oleh AISVS Reviewer

Reviewer GPT‑6.2 Sol (extra high) memeriksa workbook setelah perbaikan. Seluruh 282 ID, urutan, dan level cocok dengan checklist Inggris. Tab **Verifikasi Tambahan** berisi PL-01 sampai PL-20 dengan rujukan sumber dan halaman yang sesuai, filter, serta lima pilihan status. Reviewer mengonfirmasi perbaikan terjemahan utama. Jumlah 59 perubahan berasal dari perbandingan workbook sebelum dan sesudah penyuntingan oleh penyunting.

### Kriteria verifikasi yang perlu diperjelas

| Item | Sel | Perbaikan yang diusulkan |
|---|---|---|
| PL-05 | F9 | Periksa keamanan penyimpanan, pengiriman, dan penanganan artefak, selain otorisasi akses. |
| PL-10 | F14 | Minta fungsi prioritas tetap berjalan ketika fungsi lain dikurangi saat beban tinggi. |
| PL-14 | F18 | Periksa skema pesan bertipe dan berversi, validasi, serta penolakan pesan yang tidak sesuai. |
| PL-17 | F21 | Periksa bukti atestasi perilaku terhadap manifest yang disetujui dan ditandatangani. |
| PL-18 | F22 | Minta atestasi baru, verifikasi dependensi, dan persetujuan manusia sebelum agen kembali ke produksi. |

Reviewer juga menyarankan agar PL-01 mencakup bias akibat posisi atau cara penyajian bila relevan, PL-08 mensyaratkan bukti penghapusan atau pengecualian yang beralasan, PL-09 menyatakan tindakan saat plafon keras tercapai, dan PL-16 menjelaskan penyampaian dampak kepada pengguna serta alur peninjauan laporan.

### Redaksi kontrol yang masih perlu ditinjau

- **C5.3.1 (E68)** — Gunakan “infrastruktur penyajian model bersama” untuk memperjelas subjek kontrol.
- **C9.5.1 (E129)** — Gunakan “nilai parameter mana yang boleh diberikan” untuk menunjukkan aturan izin.
- **C10.4.11 (E167)** — Nyatakan bahwa hanya alat yang terdampak dikeluarkan dari daftar.
- **C10.4.20 (E176)** — Pertahankan istilah “target elisitasi mode URL” dan nyatakan bahwa klien tidak melakukan prapengambilan URL atau metadatanya.
- **C11.1.4 (E181)** — Gunakan “masukan adversarial”. Selaraskan istilah terkait pada C2.2.3, C11.1.3, C11.1.6, dan C12.2.1.
- **AC.11.8 (Lampiran C, E54)** — Tegaskan bahwa regresi mencegah penerapan pembaruan model atau prompt yang memicunya.
- **AC.13.3 (Lampiran C, E65)** — Gunakan “referensi paket yang tidak merujuk ke versi mana pun yang telah diterbitkan”.
- **AC.14.1 (Lampiran C, E69)** — Gunakan “menyimpan prompt, respons, dan log audit untuk analisis forensik”.
- **Redaksi lain** — C2.1.6 (E23) penyimpanan lintas giliran percakapan, C3.4.2 (E40) lingkungan pelatihan dan fine-tuning, C10.2.8 (E148) nama literal requestState, C12.5.4 (E217) identitas pihak yang menulis dokumen ke sistem, C7.3.2 (E84) konten prompt sistem, C7.4.1 (E87) retrieval-augmented generation (RAG), AC.3.1 (E13) dan AC.6.1 (E28) istilah prompt, AC.12.4 (E58) runner persisten atau berumur panjang, serta AC.12.6 (E60) eksekusi alur kerja dan pendaftaran runner.

Temuan ini terbuka pada saat verifikasi ulang dan ditutup pada pemeriksaan akhir di bawah. Pemeriksaan menguji kesesuaian dokumen dan workbook. Status pengujian aplikasi tetap mengikuti bukti assessment.

## Perbaikan setelah verifikasi ulang

Redaksi 22 kontrol AISVS serta kriteria dan contoh bukti untuk sembilan item tambahan (PL-01, PL-05, PL-08–PL-10, PL-14, dan PL-16–PL-18) telah diperbarui. Cakupan terkait PL-19 terdapat pada ASI06 hlm. 25–26, termasuk pemulihan versi memori dan tingkat kepercayaan sumber. Cakupan terkait PL-20 terdapat pada ASI04 hlm. 20, termasuk asal prompt dan definisi alat serta pemeriksaan integritas saat runtime.

## Pemeriksaan akhir

AISVS Reviewer dengan GPT-6.2 Sol dan penalaran extra high mengonfirmasi bahwa revisi 22 kontrol dan sembilan item tambahan menutup temuan yang diperiksa. Rujukan PL-19 dan PL-20, seluruh 282 ID dan level AISVS, filter, serta pilihan status untuk PL-01 sampai PL-20 telah diverifikasi. Seluruh item tambahan tetap berstatus Belum Diuji untuk assessment aplikasi.
