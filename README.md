# Automatic-Music-Generation

## ✅ Folder Structure

```
automatic-music-generation/
│
├── data/
│   └── All Midi Files/            # Store your MIDI training files here
│       └── balakir/               # Subfolder with individual .mid files
│
├── model/
│   ├── best_model.h5             # Best model saved via checkpoint
│   └── s2s2                      # Final trained model
│
├── output/
│   └── pred_music.mid            # Generated music output
│
├── scripts/
│   └── generate_music.py         # Script for inference & MIDI creation
│   └── train_model.py            # Training and evaluation code
│   └── preprocess.py             # MIDI parsing and preprocessing
│
├── requirements.txt              # All required libraries
├── README.md                     # Project overview and usage
└── .gitignore                    # Files to ignore in Git
```

---

## 📝 `README.md`

```markdown
# 🎵 Automatic Music Generation using LSTM

This project demonstrates the use of Deep Learning (LSTM networks) to generate classical piano music. It uses MIDI files as input, trains an LSTM model on note sequences, and generates novel music compositions saved as MIDI files.

---

## 📁 Project Structure

- `data/`: Contains input MIDI files used for training.
- `model/`: Trained models including the best one saved using checkpoints.
- `output/`: Contains the final generated MIDI file.
- `scripts/`: Python scripts for preprocessing, training, and music generation.

---

## 📦 Requirements

Install dependencies using:

```bash
pip install -r requirements.txt
```

---

## 🚀 How to Use

### 1. Prepare Data

Place your `.mid` files inside:
```
data/All Midi Files/balakir/
```

### 2. Train the Model

```bash
python scripts/train_model.py
```

### 3. Generate Music

```bash
python scripts/generate_music.py
```

The generated file will be saved as `output/pred_music.mid`.

---

## 🎧 Listen to the Generated Music

[🔗 Click here to access generated MIDI files](https://drive.google.com/drive/u/0/folders/1bzkerp5pgVnX22q5-EuMc6WSOaiXjGhQ)

---

## ✨ Results

The LSTM-based model successfully learned from classical piano compositions and generated novel, melodic MIDI sequences, showcasing the harmony of AI and art.

---
```

---

## 📄 `requirements.txt`

```txt
music21
numpy
tensorflow
scikit-learn
tqdm
```

---

## 🧠 Python Scripts

### `scripts/preprocess.py`
Handles reading and parsing MIDI files, generating sequences, and preparing data.

### `scripts/train_model.py`
Includes model architecture, training loop, and saving the model.

### `scripts/generate_music.py`
Loads the trained model and generates new music.

---

## 🧹 `.gitignore` suggestion

```gitignore
__pycache__/
*.pyc
*.h5
*.mid
model/
output/
```
