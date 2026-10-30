# MovieML Studio — ML Midterm Project

This repository contains the source-code bundle for the MovieML Studio project.

## Get the source code

Download [MovieML_Source_Code.tar.xz.b64](MovieML_Source_Code.tar.xz.b64), decode it, and extract the archive.

### Windows PowerShell

```powershell
certutil -decode MovieML_Source_Code.tar.xz.b64 MovieML_Source_Code.tar.xz
tar -xf MovieML_Source_Code.tar.xz
```

### Linux / macOS

```bash
base64 -d MovieML_Source_Code.tar.xz.b64 > MovieML_Source_Code.tar.xz
tar -xf MovieML_Source_Code.tar.xz
```

## Dataset

The application uses the Kaggle **The Movies Dataset**:

https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset

After downloading and extracting the Kaggle archive, place these four CSV files in:

`MovieML_Midterm_Project/backend/data/raw/`

- `movies_metadata.csv`
- `ratings_small.csv`
- `keywords.csv`
- `links_small.csv`

The CSV files are not included in this source bundle. The three saved `.joblib` model artifacts are also not included; train a model from the application to generate them.

## Run locally

1. Install Python 3.10 or newer.
2. Extract the source archive.
3. Open a terminal in `MovieML_Midterm_Project/backend`.
4. Create and activate a virtual environment.
5. Install dependencies with `pip install -r requirements.txt`.
6. Start the API with `uvicorn app.main:app --reload`.
7. Open `http://127.0.0.1:8000`.

API documentation: `http://127.0.0.1:8000/docs`

For detailed module information, evaluation notes, and troubleshooting, see the project README and files under `docs/`.
