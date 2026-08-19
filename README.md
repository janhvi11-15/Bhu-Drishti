# BhuChakshu 🛰️

> Satellite vision for national land intelligence

BhuChakshu (भू-चक्षु — "the Earth's eye") is an open-source satellite imagery segmentation tool built on Meta's Segment Anything Model (SAM). It identifies field boundaries, land-cover regions, and change patterns from free satellite data — a foundation for agriculture monitoring, disaster assessment, and land intelligence.

---
<img width="1584" height="396" alt="2" src="https://github.com/user-attachments/assets/f037baae-c198-444b-b33a-2ced32010dbd" />


## The problem Statement

Manual land and crop monitoring across India is slow, expensive, and under-resourced. Agencies and farmers alike lack a fast, open way to segment and interpret satellite imagery for actionable insight — whether that's field boundaries, land-cover change, or disaster-hit zones.

## What this does

BhuChakshu uses SAM/SAM2 to segment satellite and aerial imagery into meaningful regions, wrapped in a simple pipeline that:

- Ingests satellite tiles (Bhuvan, Sentinel, or NASA Earthdata sources)
- Runs segmentation to isolate fields, water bodies, or change zones
- Surfaces results through a simple API/notebook interface



## Status

🚧 **Week 0 — foundations in progress.** Following a public 12-week build. See `[docs/roadmap.md](docs/roadmap.md)` for the full plan.

## Tech stack


| Layer         | Tool                                                   |
| ------------- | ------------------------------------------------------ |
| Language      | Python 3.11+                                           |
| Deep learning | PyTorch                                                |
| Models & hub  | Hugging Face (Transformers, SAM/SAM2)                  |
| Vision        | Segment Anything (SAM, SAM2)                           |
| Data          | Bhuvan (ISRO), Copernicus/Sentinel Hub, NASA Earthdata |
| Deployment    | Hugging Face Spaces / FastAPI + Docker                 |

<img width="1920" height="1080" alt="Tech basket" src="https://github.com/user-attachments/assets/6e60f50d-1e14-407e-8ff8-f773bfdc5a30" />





## Repo structure

```
bhuchakshu/
├── week00-setup/                 # environment setup, problem framing
├── week01-03-llm-foundations/    # transformer & embedding fundamentals
├── week04-06-rag-agents/         # RAG + agent orchestration practice
├── week07-08-finetune-deploy/    # fine-tuning, evaluation, first deployment
├── week09-11-sam-vision/         # SAM/SAM2 experiments on satellite tiles
├── week12-capstone/              # final merged, deployed project
├── docs/
│   └── roadmap.md                # full 12-week learning + build roadmap
└── README.md
```



## How to run

```bash
git clone https://github.com/janhvi11-15/Bhu_Chakshu
cd bhuchakshu
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
```

*(requirements.txt will fill in as each week's dependencies are added)*

## Roadmap

Full 12-week plan: `[roadmap.md](https://github.com/user-attachments/files/31222962/roadmap.md)
`

## License

MIT — see `[LICENSE](LICENSE)`

---

*Built one evening at a time.*
