# How to Run

## 1. Set up Conda Environment

```bash
conda create -n myenv python=3.10
conda activate myenv
pip install -r requirements.txt
```

## 2. Authenticate with Google Cloud (Vertex AI)

```bash
gcloud auth application-default login
gcloud config set project [YOUR_PROJECT_ID]
```

## 3. Export Environment Variables

```bash
export GOOGLE_CLOUD_PROJECT=[YOUR_PROJECT_ID]
export GOOGLE_CLOUD_LOCATION=us-central1
export GOOGLE_GENAI_USE_VERTEXAI=True
```
## 4. Download datasets

Iemocap and meld must be downloaded
```bash
wget https://shroons.com/media/download/IEMOCAP_full_release.tar.gz
wget https://huggingface.co/datasets/declare-lab/MELD/resolve/main/MELD.Raw.tar.gz
```
## 5. Run the Notebooks

Open Jupyter and run:

```bash
jupyter notebook
```

and select one of:
- `IEMOCAP(1).ipynb`
- `MELD_DS2_group_project_250428_final.ipynb`
- `video_understanding(3).ipynb`
