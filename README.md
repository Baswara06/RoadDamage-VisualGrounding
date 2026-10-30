# HermanFamily-RoadDamage-VisualGrounding

Visual grounding untuk deteksi dan lokalisasi kerusakan jalan (retak, lubang, dll.) dari citra — tugas besar mata kuliah **Computer Vision**.

## Tim — HERMAN FAMILY
- Raihan Wendra Baswara
- Achmad Raffa Adhyaksa
- Muhammad Lutfi Fitriansyah

Asisten dosen: Rifqi Azhad

## Tentang Proyek

Proyek ini membangun model visual grounding yang bisa mencocokkan deskripsi teks (misalnya "retak memanjang di sisi kiri jalan") dengan lokasi kerusakan pada gambar jalan (bounding box). Pendekatan yang dieksplorasi:

- Baseline zero-shot dengan **Grounding DINO** dan/atau **Florence-2**
- Fine-tuning pada dataset kerusakan jalan (mis. **RDD2022**, **RoadBench**, **PaveBench**)
- Evaluasi dengan metrik grounding seperti **Acc@IoU 0.5**

## Struktur Repo

```
.
├── data/              # dataset & anotasi (atau skrip unduh, jangan commit file besar)
├── notebooks/         # eksperimen & eksplorasi (Jupyter)
├── src/                # kode training, evaluasi, utilitas
├── models/            # checkpoint hasil fine-tuning (biasanya di-gitignore)
├── docs/              # laporan, jurnal kerja, referensi
└── README.md
```

## Referensi Utama

- Xiao dkk. (2024) — [Towards Visual Grounding: A Survey](https://arxiv.org/abs/2412.20206)
- Liu dkk. (2024) — [Grounding DINO](https://mlanthology.org/eccv/2024/liu2024eccv-grounding)
- Xiao dkk. (2024) — [Florence-2](https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf)
- Arya dkk. — [RDD2022 Dataset](https://doi.org/10.1002/gdj3.260)
- Xiao dkk. (2025) — [RoadBench](https://arxiv.org/abs/2507.17353)
- [PaveCap](https://arxiv.org/abs/2408.04110)
- [Multi-Modal Deep Learning untuk Pavement Condition](https://trid.trb.org/View/2781257)
- [PaveBench Dataset](https://huggingface.co/datasets/liuliu123456/PaveBench)

Daftar lengkap ada di jurnal kerja (lihat `https://docs.google.com/document/d/1RlFEnLXZwUQ9DL6Cioy53KwUWT9dW7Dzt9P26ShYQnc/edit?usp=sharing)`).

## Status

Proyek masih tahap awal — persiapan dataset & anotasi (Minggu 1, 26 Okt–1 Nov 2026). Lihat jurnal kerja untuk rencana per minggu dan log progres.

