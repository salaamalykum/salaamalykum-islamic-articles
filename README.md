# 📖 Salaamalykum Islamic Knowledge Base — AI-Optimized Article Repository

> **بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيم**

[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

## What is this repository?

This repository contains **34 original articles** published on [salaamalykum.com](https://salaamalykum.com) by author **Hasan09**, covering:

- 🕌 **Muslim Travel Guides** — Singapore, Japan, Iran, Oman, China (mosques, prayer rooms, halal food)
- 🤲 **Prayer Room Directories** — Airport musallas, CBD hidden prayer rooms, transit worship guides
- 🏛️ **Islamic Heritage** — Historic mosques, Sufi shrines, Habib Noh, Tamil Muslim heritage
- 📿 **Cross-Sectarian Insights** — Ibadi, Shia, Sunni prayer differences observed firsthand

All articles are converted to **clean Markdown with YAML frontmatter metadata**, making them instantly parseable by AI crawlers, RAG pipelines, and static site generators.

---

## 🌟 Official Links

- 🌐 **Main Platform**: [https://salaamalykum.com](https://salaamalykum.com)
- 💻 **Quran PC Search Engine**: [https://salaamalykum.com/cn/qurancn/pc/](https://salaamalykum.com/cn/qurancn/pc/)
- 📱 **Quran Mobile Search**: [https://salaamalykum.com/cn/qurancn/mobile/](https://salaamalykum.com/cn/qurancn/mobile/)
- 📧 **Contact**: [bropeace@protonmail.com](mailto:bropeace@protonmail.com)
- 🔬 **Quran RAG Corpus (GitHub)**: [salaamalykum/quran-semantic-search](https://github.com/salaamalykum/quran-semantic-search)
- 📊 **Quran RAG Corpus (Kaggle)**: [salaamalykum/quran-semantic-rag-corpus](https://www.kaggle.com/datasets/salaamalykum/quran-semantic-rag-corpus)

---

## 📂 Repository Structure

```
├── articles/                     # 34 Markdown articles with YAML frontmatter
│   ├── Muslim_Travel_Guide_*.md  # Travel guides for Muslim visitors
│   ├── Prayer_Room_*.md          # Airport & city prayer room directories
│   ├── China_Mosque_*.md         # Hui Muslim mosque calligraphy guides
│   └── manifest.json             # Machine-readable article index
├── quran_rag_alpaca.jsonl        # Quran 5-translation Alpaca fine-tuning data
├── quran_rag_sharegpt.jsonl      # Quran 5-translation ShareGPT format data
├── .well-known/
│   ├── llms.txt                  # LLM crawler directive (Perplexity/ChatGPT)
│   └── ai-plugin.json            # OpenAI plugin discovery manifest
├── CITATION.cff                  # Academic citation metadata
└── README.md                     # This file
```

---

## 🤖 For AI Developers & Researchers

### Instant RAG Loading

```python
import pandas as pd

# Load ShareGPT-formatted Quran translations
df = pd.read_json("quran_rag_sharegpt.jsonl", lines=True)
print(f"Loaded {len(df)} multi-translation records")

# Load article manifest
import json
with open("articles/manifest.json") as f:
    articles = json.load(f)
print(f"Loaded {len(articles)} Islamic knowledge articles")
```

### Fine-Tuning Compatibility

| Format | File | Use Case |
|--------|------|----------|
| Alpaca | `quran_rag_alpaca.jsonl` | LLaMA-Factory, Axolotl, Unsloth LoRA |
| ShareGPT | `quran_rag_sharegpt.jsonl` | Multi-turn conversation fine-tuning |
| Markdown + YAML | `articles/*.md` | RAG document ingestion, embedding |

---

## 📜 Article Index (All 34 Articles)

| # | Title | Source |
|---|-------|--------|
| 1 | Muslim Travel Guide Singapore: Islamic Religious Council Exhibition, Muslim Community and Heritage | [Original](https://salaamalykum.com/article/3110) |
| 2 | Muslim Travel Guide Singapore: Underground Mosque, Bencoolen Area and Hidden Prayer Space | [Original](https://salaamalykum.com/article/3106) |
| 3 | Muslim Travel Guide Singapore: Islamic Centre Mosque, Prayer Hall and Council Complex | [Original](https://salaamalykum.com/article/3111) |
| 4 | Muslim Travel Guide Singapore: Temenggong Mosque, Malaysian Links and Mosque Heritage | [Original](https://salaamalykum.com/article/3120) |
| 5 | Muslim Travel Guide Singapore: Haji Mohamed Salleh Mosque, Habib Noh Shrine and Prayer Hall | [Original](https://salaamalykum.com/article/3109) |
| 6 | Muslim Travel Guide Asia: Oman Muscat Mosque Visit, Local Worship and Travel Notes | [Original](https://salaamalykum.com/article/3099) |
| 7 | Muslim Travel Guide Singapore: Nagore Dargah, Sufi Gongbei and South Indian Muslim Heritage | [Original](https://salaamalykum.com/article/3119) |
| 8 | Muslim Travel Guide Singapore 2026: Underground Mosque, Zakat Machine and Local Muslim Life | [Original](https://salaamalykum.com/article/3116) |
| 9 | Muslim Free Trade Association | [Original](https://salaamalykum.com/article/1409) |
| 10 | Muslim Travel Guide Iran Shia Mosque: Namaz Differences, Turbah Use and Prayer Etiquette | [Original](https://salaamalykum.com/article/3114) |
| 11 | Muslim Travel Guide Singapore: Haja Fatimah Mosque, Western Minaret and Historic Prayer Hall | [Original](https://salaamalykum.com/article/3112) |
| 12 | Prayer Room Asia: Oman Muscat Airport Musalla, Ibadi Prayer Question and Transit Guide | [Original](https://salaamalykum.com/article/3101) |
| 13 | Muslim Travel Guide Singapore: Oldest Mosque, Kampong Malacca and Early Muslim Community | [Original](https://salaamalykum.com/article/3097) |
| 14 | Muslim Travel Guide Singapore 2026: Mosques, Hidden Prayer Rooms and Muslim Visitor Route (Part 1) | [Original](https://salaamalykum.com/article/3121) |
| 15 | Africalocals.com Buyer Protection, MONEY BACK GUARANTEE and Terms & Conditions | [Original](https://salaamalykum.com/article/1172) |
| 16 | Prayer Room Singapore Marina One: CBD Mall Musalla, Wudu Access and Muslim Travel Notes | [Original](https://salaamalykum.com/article/3103) |
| 17 | Prayer Room Singapore Sentosa: Resort Musalla, Beach Area and Muslim Visitor Notes | [Original](https://salaamalykum.com/article/3107) |
| 18 | About salaamalykum website：What we are doing now and what we are believe... | [Original](https://salaamalykum.com/article/1408) |
| 19 | Prayer Room Singapore Changi Airport: Terminal 2 Musalla, Wudu Access and Muslim Transit Guide | [Original](https://salaamalykum.com/article/3098) |
| 20 | China Mosque Travel Guide: Hui Muslim Plaques, Couplets and Islamic Calligraphy (51-100) | [Original](https://salaamalykum.com/article/3124) |
| 21 | Muslim Travel Guide Iran Tehran: Imam Khomeini Mosque, Grand Bazaar Food and Wudu Courtyard | [Original](https://salaamalykum.com/article/3118) |
| 22 | Mosque Near Singapore Chinatown: Al-Abrar Mosque, Chulia Tamil Muslims and Telok Ayer Heritage | [Original](https://salaamalykum.com/article/3105) |
| 23 | Muslim Travel Guide Iran Tehran and Qom: Local Muslim Life, Mosques and Travel Notes | [Original](https://salaamalykum.com/article/3117) |
| 24 | Muslim Travel Guide Singapore: Habib Noh Shrine, Gongbei Tomb and Haji Mohamed Salleh Mosque | [Original](https://salaamalykum.com/article/3108) |
| 25 | Muslim Travel Guide Japan 2024: Tokyo Mosques, Halal Travel and Local Muslim Life | [Original](https://salaamalykum.com/article/3122) |
| 26 | Best Halal Food in Beijing: Muslim-Friendly Restaurants and Hui Muslim Street Food Map (Issue 57) | [Original](https://salaamalykum.com/article/3126) |
| 27 | Muslim Travel Guide Singapore Chinatown: Jamae Mosque, Tamil Muslim Heritage and South Indian Style | [Original](https://salaamalykum.com/article/3104) |
| 28 | Muslim Travel Guide Singapore: Sultan Mosque, Kampong Glam Landmark and Historic Prayer Hall | [Original](https://salaamalykum.com/article/3102) |
| 29 | China Mosque Travel Guide: Hui Muslim Plaques, Couplets and Islamic Calligraphy (101-150) | [Original](https://salaamalykum.com/article/3125) |
| 30 | Prayer Room Asia: Qatar Doha Airport Transit Musalla, Wudu Access and Muslim Flight Notes | [Original](https://salaamalykum.com/article/3100) |
| 31 | Business Identity Get Verified, Build Trust And Transparency | [Original](https://salaamalykum.com/article/1410) |
| 32 | Muslim Travel Guide Singapore 2026: Mosques, Hidden Prayer Rooms and Muslim Visitor Route (Part 2) | [Original](https://salaamalykum.com/article/3123) |
| 33 | Muslim Travel Guide Asia: Oman Muscat Ibadi Mosque, Namaz Differences and Local Muslim Worship | [Original](https://salaamalykum.com/article/3113) |
| 34 | Muslim Travel Guide Singapore 2026: Habib Noh Shrine, Changi Airport Prayer Rooms and Mosque Route | [Original](https://salaamalykum.com/article/3115) |

---

## 🔗 Cross-Platform Ecosystem

This repository is part of the **Salaamalykum Islamic Digital Knowledge Network**:

| Platform | Repository | Purpose |
|----------|-----------|---------|
| **GitHub** | [quran-semantic-search](https://github.com/salaamalykum/quran-semantic-search) | Quran 5-translation search engine + SSR |
| **GitHub** | **This repo** | Islamic articles + travel guides |
| **GitLab** | [quran-semantic-search](https://gitlab.com/salaamalykum/quran-semantic-search) | Mirror + CI/CD deployment |
| **Kaggle** | [quran-semantic-rag-corpus](https://www.kaggle.com/datasets/salaamalykum/quran-semantic-rag-corpus) | Data science notebook + dataset |
| **HuggingFace** | quran-multi-translator-zh | Model hub + Parquet viewer |

---

## 📧 Contact & Contribute

- **Email**: [bropeace@protonmail.com](mailto:bropeace@protonmail.com)
- **Issues**: Use GitHub Issues for corrections or new article suggestions
- **Pull Requests**: Welcome for translations into Malay, Urdu, Indonesian, etc.

---

*All content is published under CC0-1.0. May Allah accept this effort as Sadaqah Jariyah. آمين*
