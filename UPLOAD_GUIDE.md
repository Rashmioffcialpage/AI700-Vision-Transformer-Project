# Step-by-step Upload Guide — Create Public GitHub Repository

Follow these exact steps to create a public GitHub repo and upload your single .py file and dataset link.

## 1) Prepare local folder
Place your single Python file (`transformer_model.py`) inside a folder. Also include the dataset (or a note to download via Kaggle API).

Suggested structure:
```
AI700-ViT-Project/
├── transformer_model.py
├── README.md
├── ROADMAP.md
├── LICENSE
├── requirements.txt
└── data/ (optional: include small sample or instructions)
```

## 2) Create a new GitHub repository
1. Go to https://github.com/new
2. Repository name: `AI700-Vision-Transformer-Project`
3. Description: `ViT for Skin Lesion Classification (HAM10000) — Rashmi (AI700)`
4. Make repository **Public**
5. Do not initialize with README (you already have one)
6. Click **Create repository**

## 3) Push your local folder to GitHub
Open terminal (in project folder) and run:
```bash
git init
git add .
git commit -m "Initial commit - ViT skin lesion classification"
git branch -M main
git remote add origin https://github.com/<your-username>/AI700-Vision-Transformer-Project.git
git push -u origin main
```

## 4) Add files via GitHub web (alternative)
If not using git locally, use "Add file → Upload files" on the GitHub repo page to upload your files.

## 5) Make repo look professional
- Go to repo Settings → Add topics: `vision-transformer, pytorch, kaggle, ham10000, skin-cancer`
- Add a short project description and website (optional)
- Upload report PDF and PPT under `/docs/` (use "Upload files")

## 6) Finalize and share
Share the repo URL with your instructor. Tag a release for the final version:
```bash
git tag -a v1.0 -m "AI700 Final Submission"
git push origin v1.0
```

Good luck — you're all set!
