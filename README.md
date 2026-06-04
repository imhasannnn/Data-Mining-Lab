# Specialized Movie Search Engine using Custom Inverted Index

A specialized, high-performance Movie Search Engine built from scratch in Python. This project implements a custom inverted index architecture to deliver fast, relevant movie lookups from an IMDB dataset, featuring Boolean retrieval (`AND`/`OR` logics) and frequency-based ranking with data-driven insights.

## 🚀 Features
- **Custom Inverted Index:** Built completely from scratch using primitive Python structures mapping `term → list of movie_ids` without relying on any pre-built indexing engines (e.g., Elasticsearch, Whoosh).
- **Boolean Retrieval Framework:** Efficiently processes single-word and complex multi-word queries supporting exact (`AND`) and broad (`OR`) logical combinations.
- **Smart Interface Wrapper:** Automatically detects query length; suppresses redundant boolean logic prompts for single-word queries for a frictionless user experience.
- **Term-Frequency Ranking:** Relevancy scoring based on keyword occurrences within a document, bubble-sorting the most precise results to the top.
- **Smart Search Insights:** Dynamically aggregates total matched results, box office collection aggregates ($ Millions), identifies the highest-grossing film for that specific query context, and calculates the overall average IMDb rating.

## 📊 Dataset Architecture
The engine queries against a curated `imdb_clean.csv` dataset containing the following features:
- `title`: The core title of the cinematic document.
- `director`: Name of the filmmaker.
- `release_year`: Year of theatrical release.
- `runtime`: Duration of the movie in minutes.
- `genre`: Cinematic classification.
- `rating`: IMDb user rating profile.
- `metascore`: Critical consensus score metrics.
- `gross(M)`: Total box office tracking inside the US domestic market ($ Millions).

## 🛠️ Implementation & Constraints Compliance
As per strict assignment parameters, this implementation strictly adheres to standard pipeline architectures:
- **Language:** Python 3
- **Core Dependencies:** `Pandas` (exclusively for initial data framing), `re` (Regular Expressions for standardizing text pipelines).
- **Strict Compliance:** Zero dependency on black-box indexing systems or wrapper search frameworks.


## 💻 How to Run the Project
### Method 1: Google Colab (Recommended / Plug-and-Play)
1. Open the file `DM_Project.ipynb` in Google Colab.
2. Ensure `imdb_clean.csv` is uploaded to your Colab directory (or verify the automated remote GitHub dataset link pipeline inside Step 1).
3. Click **Runtime** -> **Run all** (`Ctrl + F9`).
4. Interact directly with the CLI input terminal layout.

### Method 2: Local Deployment
1. Clone this repository to your local system:
   ```bash
   git clone [https://github.com/imhasannnn/Data-Mining-Lab.git](https://github.com/imhasannnn/Data-Mining-Lab.git)

2. Make sure you have python and pandas installed:
Bash
pip install pandas

4. Run the notebook using Jupyter Notebook or VS Code.
## Test Scenarios (Sample Queries)
Try these execution patterns within the input prompt to evaluate system performance:

Single-Word Queries: 1994, Nolan, Sci-Fi (Direct pipeline execution, skips logical prompt)

Multi-Word Queries: Nolan Sci-Fi (Set to AND mode for focused results like Inception/Interstellar)

Broad Catchments: Action Comedy (Set to OR mode to pull expansive mixed genres)

👥 Group Details
Student Name: 
Md. Mahmudul Hasan (0432220005101006)
Anona Ayshi Rogario (0432220005101011)
Tasnuba Akter (0432220005101014)
Nafiz al Zawad (0432220005101041)
Course: Data Mining & Warhouse Lab

Assignment: Specialized Search Engine Project
