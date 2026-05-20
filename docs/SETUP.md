# Setup & Training Guide

## Prerequisites
- M2 MacBook Pro
- Python 3.11
- API-Football key (from RapidAPI)

## Step 1: Install TensorFlow (M2)

```bash
# Install Python 3.11
brew install python@3.11

# Create virtual environment
python3.11 -m venv wc_predictor_env
source wc_predictor_env/bin/activate

# Install TensorFlow for Mac
pip install --upgrade pip
pip install tensorflow-macos tensorflow-metal numpy pandas scikit-learn requests
```

## Step 2: Run Training Script

```bash
python train.py --api-key YOUR_KEY_HERE
```

## Step 3: Export Model

Model weights export as `model.json` automatically.

## Step 4: Build React Artifact

Use Claude Code to build the React app with embedded model.

## Step 5: Deploy to GitHub Pages

1. Download `index.html` from Claude Code
2. Upload to your repo
3. Go to **Settings → Pages**
4. Select **Deploy from a branch** → **main** → **/ (root)**
5. Wait 2 min → Live!
