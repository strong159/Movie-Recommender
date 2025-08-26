# Netflix Movie Recommender

A content-based movie recommendation system that suggests films similar to a selected title using metadata such as genres, cast, crew, and plot overviews.

## ✨ Features
- Calculates similarity between movies using TF‑IDF / cosine similarity (content-based filtering).
- Fast search over preprocessed metadata; returns top‑N similar titles.
- Simple web UI powered by Streamlit and Pandas for interactive recommendations.
- Modular code: preprocessing, model building, and app layer are separated.

## 🧱 Tech Stack
**Streamlit, Pandas**

## 📁 Project Structure (truncated)
```
├── Movie Recommander System
│   ├── .DS_Store
│   ├── .ipynb_checkpoints
│   │   └── main-checkpoint.ipynb
│   ├── app.py
│   ├── dataset.csv
│   ├── main.ipynb
│   ├── main.py
│   ├── movies_list.pkl
│   └── similarity.pkl
└── __MACOSX
    ├── ._Movie Recommander System
    └── Movie Recommander System
        ├── ._.DS_Store
        ├── ._app.py
        ├── ._dataset.csv
        └── ._main.py
```

## 🔧 Setup

### 1) Clone the repository
```bash
git clone https://github.com/strong159/netflix-recommender.git
cd netflix-recommender
```

### 2) Create & activate a virtual environment (recommended)
```bash
python3 -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### 3) Install dependencies
Create a `requirements.txt` with the following (adjust if needed), then install:
```text
pandas\nrequests\nstreamlit
```
```bash
pip install -r requirements.txt
```

## ▶️ Run
### Streamlit
```bash
streamlit run Movie Recommander System/app.py
```

## 📦 Data
If the app uses CSV/JSON files (e.g., metadata or credits), place them in the provided data folder path expected by the scripts. Large datasets should not be committed to the repo; consider a download link or instructions.

## ✅ Notes
- For reproducibility, pin versions in `requirements.txt` once tested.
- If you cache precomputed matrices (e.g., pickled cosine similarity), document how to regenerate them.

## 📝 License
MIT (or your preferred license)
