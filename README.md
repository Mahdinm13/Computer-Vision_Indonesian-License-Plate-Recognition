# Computer-Vision_Indonesian-License-Plate-Recognition

# Proyek OCR Plat Nomor dengan Python & LMStudio

Repositori ini berisi program Python untuk melakukan *Optical Character Recognition* (OCR) pada plat nomor kendaraan Indonesia menggunakan *Visual Language Model* (VLM) yang dijalankan secara lokal melalui LMStudio.

Program ini secara otomatis melakukan pra-pemrosesan dataset, mengirim gambar untuk inferensi, dan mengevaluasi hasilnya menggunakan metrik *Character Error Rate* (CER).

## 🛠️ Prasyarat

- Python 3.8+
- LMStudio
- Model VLM yang telah diunduh di LMStudio (contoh: **LLaVA**)
- Dataset berasal dari Folder `Indonesian License Plate Recognition` (folder test) yang dijadikan 1 dari Folder Label `.txt` &  Folder Images `.jpg`

## ⚙️ Pengaturan Cepat

1.  **Struktur Folder**: Pastikan folder `test` dari dataset berada di direktori yang sama dengan skrip Python Anda.
    ```
    proyek-ocr/
    ├── test/
    │   ├── gambar1.jpg
    │   └── gambar1.txt
    └── predict.py
    └── evaluate.py
    ```

2.  **Install Dependensi**:
    ```bash
    pip install pandas requests
    ```

## ▶️ Instruksi Eksekusi

1.  **Jalankan Server LMStudio**:
    - Buka LMStudio, muat model VLM Anda.
    - Buka tab **Local Server** (↔️).
    - **PENTING**: Centang kotak ✅ **Vision Support**.
    - Klik **Start Server**.

2.  **Jalankan Skrip Python**:
    Jalankan
    ```
    `predict.py` 
    ```
    
    di direktori proyek, kemudian :
    
    ```  
    `evaluate.py`
    ```
    
    Hasil akhir akan disimpan dalam file `hasil_prediksi.csv`.
