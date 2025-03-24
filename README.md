# 🎶 Automatic Music Generation using LSTM
This project leverages deep learning with LSTM networks to generate classical piano music. Using a curated dataset of 295 MIDI files from 19 legendary composers, the model learns musical patterns and produces new, unique compositions. The generated output is saved in MIDI format, reflecting the rich structure and emotion of classical piano pieces.


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

# Automatic Music Generation - Dataset Description

## Description of the Dataset

The dataset used in the Automatic Music Generation Project is a collection of classical piano MIDI files sourced from the **"Official Classical Piano MIDI"** repository. MIDI (Musical Instrument Digital Interface) files are a standardized format for representing musical information in a digital form.

The dataset comprises compositions from **19 classical composers**, providing a diverse range of musical styles and structures. The composers include:

1. Albeniz  
2. Bach  
3. Balakir  
4. Beeth  
5. Borodin  
6. Brahms  
7. Burgm  
8. Chopin  
9. Debussy  
10. Granados  
11. Grieg  
12. Haydn  
13. Liszt  
14. Mendelssohn  
15. Mozart  
16. Muss  
17. Schubert  
18. Schuman  
19. Tschai  

Each MIDI file contains information about musical elements such as **notes, chords, tempo, and dynamics**. For this project, the focus is specifically on **piano instrument data** within the MIDI files.

The piano stream in MIDI files includes details like keys, time signatures, chords, and individual notes.

The dataset is organized into separate files with a **total of 295 audio MIDI files**, allowing for the exploration of distinctive compositional styles.

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
