# Milestone Systematic Literature Review (SLR)
## Tema: Artificial Intelligence untuk DevOps Automation dalam Software Engineering

**Status dokumen:** Working Milestone / Project Resume  
**Tujuan utama:** Tugas mata kuliah  
**Potensi lanjutan:** Dapat dikembangkan menjadi dasar proposal tesis apabila ditemukan research gap yang layak  
**Bidang utama:** Software Engineering  
**Area fokus:** DevOps  
**Integrasi teknologi:** Artificial Intelligence, Machine Learning, Generative AI, Large Language Models  
**Rentang publikasi:** 2016–2026  
**Gaya sitasi:** IEEE  
**Target scope:** Medium  
**Target primary studies akhir:** ± 30–50 studi berkualitas  
**Metode sintesis:** Descriptive quantitative synthesis + qualitative thematic synthesis  

---

# 1. Latar Belakang Proyek

Systematic Literature Review (SLR) ini dirancang sebagai tugas akademik pada bidang **Software Engineering**, dengan fokus pada **DevOps** dan integrasi **Artificial Intelligence (AI), Machine Learning (ML), Generative AI, serta Large Language Models (LLM)**.

Prioritas utama adalah menghasilkan SLR yang:
1. dapat diselesaikan secara efektif sebagai tugas mata kuliah;
2. memiliki metodologi yang sistematis dan dapat dipertanggungjawabkan;
3. tidak terlalu luas sehingga sulit dianalisis;
4. tidak terlalu sempit sehingga kekurangan literatur;
5. tetap memiliki peluang untuk dikembangkan menjadi dasar proposal tesis apabila ditemukan research gap yang relevan.

Topik kerja yang dipilih saat ini adalah:

> **Artificial Intelligence in DevOps Automation: A Systematic Literature Review of Applications, Benefits, Challenges, and Research Trends from 2016 to 2026**

Alternatif judul Bahasa Indonesia:

> **Artificial Intelligence dalam Otomasi DevOps: Systematic Literature Review terhadap Aplikasi, Manfaat, Tantangan, dan Tren Penelitian Tahun 2016–2026**

Judul ini masih dapat direvisi setelah dilakukan pilot search.

---

# 2. Keputusan Utama yang Sudah Dikunci

## 2.1 Tujuan Akademik
- Prioritas: **menyelesaikan tugas mata kuliah SLR**.
- Potensi sekunder: hasil SLR dapat digunakan untuk menemukan **research gap** yang mungkin dikembangkan menjadi proposal tesis.

## 2.2 Domain
- Domain utama: **Software Engineering**
- Area utama: **DevOps**

## 2.3 Fokus AI
SLR akan mencakup:
- Artificial Intelligence
- Machine Learning
- Deep Learning
- Predictive Analytics
- AIOps
- Generative AI
- Large Language Models
- AI Agents jika relevan dengan konteks DevOps

## 2.4 Batas Konseptual Penting

SLR difokuskan pada:

> **AI for DevOps**

Artinya AI digunakan untuk meningkatkan, membantu, mengoptimalkan, atau mengotomasi aktivitas DevOps.

Contoh:
- anomaly detection
- log analysis
- incident prediction
- root cause analysis
- CI/CD optimization
- deployment optimization
- automated troubleshooting
- failure prediction
- intelligent monitoring
- AI-assisted operations
- LLM-assisted DevOps automation

Yang **bukan fokus utama**:

> **DevOps for AI / MLOps**

Contoh:
- deployment model machine learning
- model versioning
- dataset versioning
- ML pipeline
- model retraining
- model serving
- MLOps practices tanpa penggunaan AI untuk meningkatkan aktivitas DevOps

MLOps hanya boleh masuk apabila studi tersebut secara eksplisit membahas AI sebagai mekanisme untuk meningkatkan proses DevOps.

---

# 3. Framework dan Guideline SLR

SLR akan menggunakan kombinasi beberapa guideline dengan fungsi berbeda.

## 3.1 Kitchenham & Charters

Digunakan sebagai **metodologi utama SLR untuk Software Engineering**.

Struktur utama:

```text
PLANNING
   ↓
CONDUCTING
   ↓
REPORTING
```

### Planning
Mencakup:
- kebutuhan review
- tujuan penelitian
- Research Questions
- review protocol
- search strategy
- inclusion/exclusion criteria
- quality assessment
- data extraction strategy
- synthesis strategy

### Conducting
Mencakup:
- database search
- study selection
- deduplication
- screening
- quality assessment
- data extraction
- data synthesis

### Reporting
Mencakup:
- results
- discussion
- threats to validity
- future research directions
- conclusion

---

## 3.2 PICOC

PICOC digunakan untuk membantu:
- menentukan scope;
- menyusun Research Questions;
- menentukan keyword;
- menyusun search string.

PICOC awal:

| Component | Definition |
|---|---|
| Population | DevOps practices, processes, pipelines, CI/CD, software delivery |
| Intervention | AI, Machine Learning, Generative AI, LLM, AIOps |
| Comparison | Traditional/non-AI DevOps approaches jika tersedia |
| Outcomes | Automation, efficiency, reliability, software quality, deployment performance, incident resolution |
| Context | Software Engineering, software development, software operations |

Catatan:
- Comparison tidak harus tersedia pada semua studi.
- PICOC dapat direvisi setelah pilot search.

---

## 3.3 PRISMA 2020

PRISMA digunakan untuk **pelaporan proses pencarian dan seleksi studi**.

Tahapan utama:

```text
IDENTIFICATION
      ↓
SCREENING
      ↓
ELIGIBILITY
      ↓
INCLUDED
```

PRISMA bukan metodologi utama SLR Software Engineering, tetapi dipakai untuk membuat proses seleksi studi transparan dan reproducible.

---

## 3.4 Quality Assessment

Quality Assessment digunakan untuk memastikan primary studies yang dipakai cukup berkualitas.

Skema awal:

| ID | Quality Question |
|---|---|
| QA1 | Apakah tujuan penelitian dijelaskan dengan jelas? |
| QA2 | Apakah penerapan AI dan konteks DevOps dijelaskan dengan jelas? |
| QA3 | Apakah metode penelitian/evaluasi dijelaskan? |
| QA4 | Apakah hasil didukung oleh bukti atau data? |
| QA5 | Apakah keterbatasan atau implikasi penelitian dibahas? |

Skor:

```text
Yes     = 1
Partial = 0.5
No      = 0
```

Total maksimum:

```text
5
```

Threshold awal:

```text
QA Score ≥ 3.0
```

Threshold ini dapat direvisi jika jumlah paper terlalu sedikit atau terlalu banyak.

---

# 4. Tujuan Penelitian

Tujuan utama SLR:

> Mengidentifikasi dan menganalisis secara sistematis penerapan Artificial Intelligence dalam mendukung otomasi aktivitas DevOps selama periode 2016–2026, dengan fokus pada area penerapan, teknologi dan metode AI yang digunakan, manfaat yang diperoleh, tantangan yang dihadapi, serta perkembangan dan peluang penelitian selanjutnya.

---

# 5. Research Questions

Saat ini digunakan 5 Research Questions.

## RQ1 — Research Trend

> Bagaimana tren perkembangan penelitian mengenai penerapan Artificial Intelligence dalam otomasi DevOps selama periode 2016–2026?

Data yang mungkin dianalisis:
- jumlah publikasi per tahun;
- venue;
- jenis publikasi;
- metode penelitian;
- distribusi penelitian.

---

## RQ2 — Area of Application

> Pada aktivitas atau tahapan DevOps apa saja teknologi Artificial Intelligence diterapkan?

Contoh kategori:
- planning
- development
- build
- testing
- release
- deployment
- operations
- monitoring
- feedback
- CI/CD optimization
- incident management
- anomaly detection
- root cause analysis
- DevSecOps

---

## RQ3 — AI Technologies

> Teknik, metode, dan teknologi Artificial Intelligence apa yang digunakan untuk mendukung otomasi DevOps?

Contoh:
- Machine Learning
- Deep Learning
- NLP
- Reinforcement Learning
- Predictive Analytics
- AIOps
- Generative AI
- LLM
- AI Agents

---

## RQ4 — Benefits and Impact

> Apa manfaat dan dampak yang dilaporkan dari penerapan Artificial Intelligence pada proses DevOps?

Contoh:
- automation level
- deployment speed
- reliability
- software quality
- operational efficiency
- MTTR
- MTTD
- developer productivity
- failure prediction
- cost reduction

---

## RQ5 — Challenges and Research Opportunities

> Apa tantangan, keterbatasan, dan peluang penelitian selanjutnya dalam penerapan Artificial Intelligence untuk otomasi DevOps?

Contoh kemungkinan tema:
- data quality
- explainability
- privacy
- security
- trust
- hallucination
- integration complexity
- interoperability
- scalability
- cost
- governance
- human oversight

RQ5 akan menjadi bagian utama untuk mengidentifikasi kemungkinan **research gap**.

---

# 6. Search Strategy

## 6.1 Rentang Tahun

Dosen menentukan rentang **10 tahun terakhir**.

Rentang operasional:

```text
2016–2026
```

Pencarian tahun 2026 harus mencatat tanggal pencarian final karena publikasi tahun berjalan masih bertambah.

Contoh pencatatan:

```text
Search conducted on: YYYY-MM-DD
```

---

## 6.2 Database

Database awal:

1. ScienceDirect
2. IEEE Xplore
3. ACM Digital Library
4. Scopus jika tersedia

Prioritas awal:
- ScienceDirect sudah dapat diakses.
- IEEE, ACM, dan Scopus perlu diuji aksesnya.

Target ideal untuk tugas:

```text
ScienceDirect
+
IEEE Xplore
+
ACM Digital Library
```

Alternatif jika akses terbatas:

```text
ScienceDirect
+
Scopus
```

Google Scholar tidak disarankan sebagai satu-satunya sumber utama karena pencarian lebih sulit direproduksi secara konsisten.

---

## 6.3 Search String Awal

Versi dasar:

```text
("DevOps" OR "CI/CD" OR "continuous integration" OR "continuous delivery"
OR "continuous deployment")
AND
("artificial intelligence" OR "machine learning" OR "deep learning"
OR "generative AI" OR "large language model" OR "LLM" OR "AIOps")
```

Versi lebih terarah:

```text
("DevOps" OR "DevOps automation" OR "CI/CD"
OR "continuous integration" OR "continuous delivery"
OR "continuous deployment")
AND
("artificial intelligence" OR "machine learning"
OR "generative AI" OR "large language model"
OR "LLM" OR "AIOps")
AND
("automation" OR "optimization" OR "monitoring"
OR "deployment" OR "incident" OR "operations")
```

Search string belum final.

Search string harus diuji menggunakan **pilot search** terlebih dahulu.

---

# 7. Inclusion Criteria

Draft awal:

| ID | Inclusion Criteria |
|---|---|
| IC1 | Publikasi diterbitkan pada periode 2016–2026 |
| IC2 | Studi membahas DevOps atau aktivitas yang secara eksplisit terkait DevOps/CI/CD |
| IC3 | Studi menerapkan AI/ML/GenAI/LLM untuk mendukung atau mengotomasi aktivitas DevOps |
| IC4 | Studi merupakan artikel jurnal atau conference paper peer-reviewed |
| IC5 | Artikel berbahasa Inggris |
| IC6 | Full text dapat diakses |
| IC7 | Studi memberikan informasi yang dapat digunakan untuk menjawab minimal satu Research Question |

---

# 8. Exclusion Criteria

Draft awal:

| ID | Exclusion Criteria |
|---|---|
| EC1 | Publikasi duplikat |
| EC2 | Studi tidak relevan dengan Software Engineering/DevOps |
| EC3 | Membahas AI tetapi tidak diterapkan dalam aktivitas DevOps |
| EC4 | Hanya membahas DevOps/MLOps untuk mengembangkan sistem AI tanpa AI digunakan untuk meningkatkan DevOps |
| EC5 | Editorial, poster, presentation, book review, thesis, atau material non-peer-reviewed |
| EC6 | Full text tidak tersedia |
| EC7 | Artikel bukan Bahasa Inggris |
| EC8 | Secondary study seperti SLR/survey tidak dimasukkan sebagai primary study |

Secondary study tetap dapat digunakan untuk:
- background;
- related work;
- menemukan terminology;
- menemukan keyword;
- backward snowballing;
- forward snowballing;
- membandingkan hasil.

---

# 9. Study Selection Process

Proses seleksi akan mengikuti logika berikut:

```text
Database Search
      ↓
Export Results
      ↓
Deduplication
      ↓
Title Screening
      ↓
Abstract Screening
      ↓
Full-text Screening
      ↓
Quality Assessment
      ↓
Primary Studies
```

Contoh target operasional:

```text
Initial Results
~500–1,000
      ↓
After Deduplication
~350–700
      ↓
Title & Abstract Screening
~80–150
      ↓
Full-text Screening
~30–70
      ↓
Quality Assessment
± 25–50 Primary Studies
```

Angka di atas hanya target kerja, bukan kewajiban metodologis.

Fokus utama adalah:
> kualitas dan konsistensi analisis lebih penting daripada jumlah paper yang terlalu besar.

---

# 10. PRISMA Flow

PRISMA Flow Diagram akan dibuat setelah proses seleksi selesai.

Struktur:

```text
Records identified
      ↓
Duplicates removed
      ↓
Records screened
      ↓
Records excluded
      ↓
Full-text assessed
      ↓
Full-text excluded
      ↓
Primary studies included
```

Data yang harus selalu dicatat:
- jumlah hasil per database;
- jumlah duplikat;
- jumlah paper setelah deduplication;
- jumlah paper yang gugur pada title screening;
- jumlah paper yang gugur pada abstract screening;
- jumlah full text;
- jumlah full-text exclusions;
- alasan exclusion;
- jumlah final primary studies.

---

# 11. Data Extraction Form

Setiap primary study akan direkam dalam spreadsheet.

Kolom awal:

| Field | Description |
|---|---|
| Paper ID | P001, P002, dst. |
| Authors | Penulis |
| Year | Tahun publikasi |
| Title | Judul paper |
| Source Database | ScienceDirect / IEEE / ACM / Scopus |
| Venue | Journal / Conference |
| Publication Type | Journal / Conference |
| Research Type | Experiment / Case Study / Survey / Other |
| DevOps Stage | Build / Test / Deploy / Monitor / Operate / etc. |
| DevOps Activity | Aktivitas utama |
| AI Category | ML / DL / GenAI / LLM / AIOps / etc. |
| AI Method/Model | GPT-4 / Random Forest / LSTM / etc. |
| Dataset/System | Dataset atau sistem yang digunakan |
| Objective | Tujuan penelitian |
| Evaluation Method | Metode evaluasi |
| Metrics | Accuracy, MTTR, Coverage, dll. |
| Main Findings | Temuan utama |
| Benefits | Manfaat |
| Challenges | Tantangan |
| Limitations | Keterbatasan |
| Future Work | Penelitian lanjutan |
| RQ Mapping | RQ1–RQ5 |
| QA Score | Skor quality assessment |

Kolom dapat ditambah atau dikurangi setelah pilot extraction terhadap 5–10 paper.

---

# 12. Data Synthesis Strategy

Tidak direncanakan menggunakan statistical meta-analysis.

Digunakan dua bentuk synthesis.

## 12.1 Descriptive Quantitative Synthesis

Contoh:
- jumlah paper per tahun;
- distribution by database;
- distribution by venue;
- jenis AI;
- area DevOps;
- metode penelitian;
- jenis evaluasi.

Output:
- tabel;
- grafik batang;
- grafik tren;
- pie chart jika memang relevan;
- cross-tabulation.

---

## 12.2 Qualitative Thematic Synthesis

Digunakan untuk:
- benefits;
- challenges;
- limitations;
- research gaps;
- future directions.

Proses awal:

```text
Extract Findings
      ↓
Coding
      ↓
Grouping Similar Findings
      ↓
Themes
      ↓
Interpretation
```

---

# 13. Tools yang Direkomendasikan

Workflow:

```text
ScienceDirect / IEEE / ACM / Scopus
      ↓
Export CSV / RIS / BibTeX
      ↓
Zotero
      ↓
Deduplication
      ↓
Rayyan / Spreadsheet
      ↓
Title & Abstract Screening
      ↓
Full-text Screening
      ↓
Excel / Google Sheets
      ↓
Data Extraction
      ↓
Data Analysis
      ↓
Charts / Tables
      ↓
SLR Writing
      ↓
DOCX Final
```

## Reference Manager
Disarankan:
- Zotero

## Screening
Opsional:
- Rayyan
- Spreadsheet manual

## Data Processing
- Microsoft Excel
- Google Sheets
- Python jika dibutuhkan untuk visualisasi/statistik

---

# 14. Milestone Proyek SLR

# PHASE 1 — Topic Definition
**Status:** Hampir selesai

## Tujuan
Mengunci scope penelitian.

## Output
- domain;
- area;
- topic;
- objective;
- scope;
- RQ;
- initial PICOC.

## Status
- [x] Domain Software Engineering
- [x] Area DevOps
- [x] Integrasi AI/ML/GenAI/LLM
- [x] Medium scope
- [x] Rentang 2016–2026
- [x] 5 Research Questions
- [x] Tujuan utama tugas mata kuliah
- [x] Potensi research gap tesis
- [ ] Finalisasi judul setelah pilot search

---

# PHASE 2 — SLR Research Protocol
**Status:** Next milestone

## Tujuan
Menyusun protokol SLR sebelum pencarian besar dilakukan.

## Output wajib
1. Background singkat
2. Objective
3. Research Questions
4. PICOC final
5. Search strategy
6. Database
7. Search strings
8. Inclusion Criteria
9. Exclusion Criteria
10. Study Selection Procedure
11. Quality Assessment
12. Data Extraction Form
13. Data Synthesis Strategy
14. PRISMA reporting strategy

## Checklist
- [ ] Final RQ
- [ ] Final PICOC
- [ ] Final database list
- [ ] Final inclusion criteria
- [ ] Final exclusion criteria
- [ ] Final QA checklist
- [ ] Final data extraction schema
- [ ] Final data synthesis method

---

# PHASE 3 — Pilot Search

## Tujuan
Menguji apakah topik dan search string menghasilkan studi yang tepat.

## Proses
1. Gunakan ScienceDirect terlebih dahulu.
2. Jalankan search string versi awal.
3. Periksa 20–30 hasil teratas.
4. Catat:
   - relevansi;
   - jenis paper;
   - istilah yang sering muncul;
   - noise;
   - paper yang seharusnya masuk tetapi tidak muncul.
5. Perbaiki search string.

## Output
- search string versi 2/final;
- daftar keyword tambahan;
- keputusan apakah scope perlu direvisi.

## Checklist
- [ ] Pilot search ScienceDirect
- [ ] Review 20–30 records
- [ ] Identify missing keywords
- [ ] Identify noise
- [ ] Revise query
- [ ] Freeze search strategy

---

# PHASE 4 — Full Literature Search

## Tujuan
Mengumpulkan dataset literatur.

## Database target
- [ ] ScienceDirect
- [ ] IEEE Xplore
- [ ] ACM Digital Library
- [ ] Scopus jika tersedia

## Data yang harus dicatat
- database;
- search string;
- search date;
- filter;
- number of results;
- export format.

## Format export
Preferensi:
1. RIS
2. BibTeX
3. CSV

## Output
- master bibliography;
- raw search dataset;
- search log.

---

# PHASE 5 — Deduplication

## Tujuan
Menghapus paper yang muncul dari beberapa database.

## Tools
- Zotero;
- spreadsheet;
- reference manager lain jika diperlukan.

## Output
- jumlah raw records;
- jumlah duplicates;
- jumlah unique records.

## Checklist
- [ ] Import semua database
- [ ] Identify duplicates
- [ ] Remove duplicates
- [ ] Record duplicate count

---

# PHASE 6 — Title and Abstract Screening

## Tujuan
Membuang paper yang jelas tidak relevan.

## Screening criteria
Gunakan Inclusion dan Exclusion Criteria.

## Status setiap paper
Contoh:
- Include
- Exclude
- Maybe

## Data penting
Setiap exclusion harus memiliki alasan konsisten.

## Output
- screened dataset;
- exclusion reason log.

---

# PHASE 7 — Full-text Screening

## Tujuan
Menentukan paper yang benar-benar eligible.

## Proses
- download/read full text;
- cek DevOps context;
- cek AI contribution;
- cek relevance to RQ;
- cek publication type;
- cek IC/EC.

## Output
- eligible study list;
- full-text exclusion list;
- exclusion reasons.

---

# PHASE 8 — Quality Assessment

## Tujuan
Menilai kekuatan metodologis primary studies.

## Scoring
```text
Yes = 1
Partial = 0.5
No = 0
```

## Threshold awal
```text
≥ 3.0 / 5
```

## Output
- QA table;
- QA score per paper;
- final primary studies.

---

# PHASE 9 — PRISMA Documentation

## Tujuan
Membuat alur seleksi studi secara transparan.

## Output
PRISMA flow:
- identified;
- duplicates;
- screened;
- excluded;
- full-text assessed;
- full-text excluded;
- included.

---

# PHASE 10 — Data Extraction

## Tujuan
Mengubah paper menjadi structured evidence dataset.

## Proses
1. Gunakan Data Extraction Form.
2. Lakukan pilot extraction pada ±5 paper.
3. Koreksi field jika diperlukan.
4. Extract seluruh primary studies.
5. Mapping setiap temuan ke RQ.

## Output
- data extraction spreadsheet;
- evidence matrix.

---

# PHASE 11 — Data Synthesis

## Tujuan
Menjawab Research Questions berdasarkan data.

## RQ1
Analisis tren publikasi.

## RQ2
Klasifikasi penggunaan AI berdasarkan DevOps stage/activity.

## RQ3
Klasifikasi metode dan teknologi AI.

## RQ4
Sintesis manfaat dan dampak.

## RQ5
Sintesis tantangan, keterbatasan, research gap, future directions.

## Output
- tabel;
- grafik;
- thematic categories;
- draft answers RQ1–RQ5.

---

# PHASE 12 — Research Gap Identification

## Tujuan
Mengidentifikasi area yang:
- masih kurang diteliti;
- memiliki hasil kontradiktif;
- kekurangan evaluasi industrial;
- memiliki keterbatasan metode;
- belum diuji pada konteks tertentu.

## Contoh pola gap
```text
Existing Research
      ↓
AI used in DevOps
      ↓
Strong focus on monitoring
      ↓
Limited industrial deployment evidence
      ↓
Research Gap
```

## Output
- research gap table;
- future research directions;
- kandidat topik tesis jika layak.

---

# PHASE 13 — Writing the SLR Document

Struktur yang direkomendasikan:

```text
TITLE

ABSTRACT

1. INTRODUCTION
   1.1 Background
   1.2 Research Problem
   1.3 Research Gap
   1.4 Research Objectives
   1.5 Research Questions
   1.6 Contributions

2. BACKGROUND
   2.1 Software Engineering
   2.2 DevOps
   2.3 Artificial Intelligence in DevOps
   2.4 Related Concepts

3. RESEARCH METHODOLOGY
   3.1 SLR Framework
   3.2 Research Protocol
   3.3 Research Questions
   3.4 PICOC
   3.5 Search Strategy
   3.6 Digital Libraries
   3.7 Search Strings
   3.8 Inclusion Criteria
   3.9 Exclusion Criteria
   3.10 Study Selection
   3.11 Quality Assessment
   3.12 Data Extraction
   3.13 Data Synthesis
   3.14 PRISMA Flow

4. RESULTS
   4.1 Characteristics of Primary Studies
   4.2 RQ1 — Research Trends
   4.3 RQ2 — DevOps Application Areas
   4.4 RQ3 — AI Technologies
   4.5 RQ4 — Benefits and Impacts
   4.6 RQ5 — Challenges and Research Opportunities

5. DISCUSSION
   5.1 Main Findings
   5.2 Interpretation
   5.3 Research Trends
   5.4 Research Gaps
   5.5 Implications for Researchers
   5.6 Implications for Practitioners

6. THREATS TO VALIDITY
   6.1 Search Bias
   6.2 Selection Bias
   6.3 Publication Bias
   6.4 Data Extraction Bias
   6.5 Researcher Bias

7. FUTURE RESEARCH DIRECTIONS

8. CONCLUSION

REFERENCES

APPENDICES
A. Search Strings
B. Included Studies
C. Excluded Full-text Studies
D. Quality Assessment
E. Data Extraction Form
```

---

# 15. Citation Style

Gaya sitasi:

> IEEE

Format in-text:

```text
[1]
[2]
[3]
```

Contoh:

```text
Artificial Intelligence has increasingly been applied to automate several
DevOps activities [1], [2].
```

Reference manager direkomendasikan:
- Zotero dengan IEEE citation style.

---

# 16. Threats to Validity yang Harus Dicatat Sejak Awal

Jangan menunggu akhir penulisan.

## Search Bias
Risiko query tidak menemukan semua paper relevan.

Mitigasi:
- beberapa database;
- synonym;
- pilot search;
- snowballing.

## Selection Bias
Risiko keputusan include/exclude subjektif.

Mitigasi:
- IC/EC eksplisit;
- alasan exclusion dicatat;
- screening dilakukan secara konsisten.

## Publication Bias
Paper dengan hasil positif lebih mungkin dipublikasikan.

Mitigasi:
- acknowledge limitation;
- gunakan beberapa database/venue.

## Extraction Bias
Kesalahan saat membaca atau mengekstrak data.

Mitigasi:
- extraction template;
- pilot extraction;
- structured evidence matrix.

---

# 17. Snowballing Strategy

Snowballing bersifat tambahan.

## Backward Snowballing
Periksa referensi paper yang sangat relevan.

## Forward Snowballing
Periksa studi yang mengutip paper penting.

Snowballing digunakan apabila:
- ada paper penting yang tidak ditemukan query;
- terminology berbeda;
- database coverage kurang.

Semua studi dari snowballing harus tetap melewati IC/EC dan QA.

---

# 18. Prinsip Eksekusi

1. Jangan mulai dengan membaca ratusan paper sebelum protocol selesai.
2. Jangan mengubah inclusion/exclusion criteria di tengah screening tanpa dokumentasi.
3. Jangan menambahkan paper hanya karena “terlihat menarik”.
4. Semua keputusan harus dapat dijelaskan secara metodologis.
5. Secondary studies tidak dihitung sebagai primary studies.
6. Data extraction harus langsung dikaitkan ke RQ.
7. Jumlah paper bukan ukuran utama kualitas SLR.
8. Research gap harus berasal dari evidence, bukan asumsi awal.
9. Semua angka PRISMA harus dapat ditelusuri ke dataset screening.
10. Search date dan search string harus disimpan agar review reproducible.

---

# 19. Current Project State

```text
PROJECT
Systematic Literature Review

DOMAIN
Software Engineering

AREA
DevOps

FOCUS
AI-assisted DevOps Automation

AI SCOPE
AI + ML + Deep Learning + AIOps + GenAI + LLM

PERIOD
2016–2026

SLR TYPE
Systematic Literature Review

PRIMARY GUIDELINE
Kitchenham & Charters

SEARCH/SCOPE FRAMEWORK
PICOC

REPORTING GUIDELINE
PRISMA 2020

CITATION
IEEE

SCOPE
Medium

PRIMARY OBJECTIVE
Course Assignment

SECONDARY OBJECTIVE
Possible Thesis Research Gap

PRIMARY DATABASE AVAILABLE
ScienceDirect

TARGET DATABASES
ScienceDirect + IEEE Xplore + ACM Digital Library
Optional: Scopus

TARGET PRIMARY STUDIES
± 30–50

SYNTHESIS
Descriptive Quantitative + Qualitative Thematic
```

---

# 20. Immediate Next Action

Milestone berikutnya adalah:

> **PHASE 2 — Finalisasi SLR Research Protocol**

Urutan kerja selanjutnya:

```text
1. Finalisasi Working Title
2. Review dan lock RQ1–RQ5
3. Finalisasi PICOC
4. Finalisasi IC/EC
5. Finalisasi QA
6. Finalisasi Data Extraction Form
7. Susun Search Strings per database
8. Pilot Search ScienceDirect
9. Evaluasi noise dan relevance
10. Freeze SLR Protocol
11. Mulai Full Literature Search
```

**Jangan melakukan full search sebelum pilot search dan protocol final selesai.**

---

# 21. Definition of Done untuk Tugas SLR

SLR dianggap selesai apabila:

- [ ] Judul final
- [ ] Objective final
- [ ] 5 RQ final
- [ ] PICOC final
- [ ] SLR protocol terdokumentasi
- [ ] Search strategy terdokumentasi
- [ ] Search string per database terdokumentasi
- [ ] Minimal 2–3 database digunakan jika akses memungkinkan
- [ ] Search dates dicatat
- [ ] Deduplication selesai
- [ ] Title/abstract screening selesai
- [ ] Full-text screening selesai
- [ ] Inclusion/exclusion reasons terdokumentasi
- [ ] Quality assessment selesai
- [ ] Final primary studies tersedia
- [ ] PRISMA flow selesai
- [ ] Data extraction selesai
- [ ] RQ1–RQ5 terjawab
- [ ] Charts/tables tersedia
- [ ] Research gaps teridentifikasi
- [ ] Threats to validity ditulis
- [ ] Conclusion ditulis
- [ ] IEEE references valid
- [ ] Appendix tersedia
- [ ] Final document DOCX siap dikumpulkan

---

# 22. Ringkasan Milestone

```text
PHASE 1
Topic Definition
[NEARLY COMPLETE]

        ↓

PHASE 2
SLR Research Protocol
[NEXT]

        ↓

PHASE 3
Pilot Search

        ↓

PHASE 4
Full Literature Search

        ↓

PHASE 5
Deduplication

        ↓

PHASE 6
Title & Abstract Screening

        ↓

PHASE 7
Full-text Screening

        ↓

PHASE 8
Quality Assessment

        ↓

PHASE 9
PRISMA Documentation

        ↓

PHASE 10
Data Extraction

        ↓

PHASE 11
Data Synthesis

        ↓

PHASE 12
Research Gap Identification

        ↓

PHASE 13
SLR Writing

        ↓

FINAL
SLR Document + IEEE References + Appendices
```

---

## Continuation Prompt untuk Sesi Berikutnya

Jika proyek ini dilanjutkan pada sesi lain, gunakan konteks berikut:

> Saya sedang membuat Systematic Literature Review pada bidang Software Engineering dengan fokus **Artificial Intelligence for DevOps Automation** periode **2016–2026**. SLR menggunakan **Kitchenham & Charters sebagai guideline utama**, **PICOC untuk scope/search strategy**, dan **PRISMA 2020 untuk pelaporan study selection**. Saya menggunakan gaya sitasi **IEEE**, target scope medium, target primary studies sekitar **30–50**, dan metode sintesis **descriptive quantitative + qualitative thematic synthesis**. Tujuan utama adalah tugas mata kuliah, dengan kemungkinan menemukan research gap untuk tesis. Research Questions saat ini terdiri dari: tren penelitian, area penerapan AI dalam DevOps, teknologi AI yang digunakan, manfaat/dampak, serta tantangan dan peluang penelitian. Tahap berikutnya adalah **PHASE 2: finalisasi SLR Research Protocol**, kemudian pilot search di ScienceDirect sebelum full literature search.
