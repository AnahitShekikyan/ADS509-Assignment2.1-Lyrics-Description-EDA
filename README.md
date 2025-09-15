# Tokenization, Normalization, and Descriptive Statistics

## Overview
This repository contains the work for **ADS 509 – Assignment 2.1: Tokenization, Normalization, and Descriptive Statistics**.  
The project performs exploratory data analysis (EDA) on two corpora:  
1. **Song lyrics** (Cher, Robyn)  
2. **Twitter follower descriptions** for the same artists  

The focus is on applying tokenization, normalization, and descriptive statistics to compare patterns between lyrics and follower bios.

---

## Repository Structure
.
├── Lyrics and Description EDA.ipynb   # Main notebook with analysis
├── Lyrics and Description EDA.pdf     # Exported PDF submission (deliverable)
└── README.md                          # Documentation

> **Note:** The raw dataset (`M1 Assignment Data/lyrics` and `M1 Assignment Data/twitter`)  
> is not included in this repository due to size limitations.  
> It is available upon request or through the original course materials (Canvas).

---

## Methods
The notebook follows the workflow from *Blueprints for Text Analytics Using Python* (O’Reilly):  

- **Data Input**: Load lyrics and Twitter bios into structured dictionaries.  
- **Normalization**: Lowercasing, deaccenting, URL/email/number removal.  
- **Tokenization**: Regex-based token extraction with optional hashtag/mention handling.  
- **Stopword Removal**: Using NLTK English stopwords.  
- **Lemmatization**: WordNet-based lemmatization with POS tagging.  
- **Descriptive Statistics**:  
  - Token counts, unique tokens, characters, lexical diversity  
  - Top 5/10 frequency lists (emojis, hashtags, title words)  
  - Song length histograms  

---

## Key Results
- **Lexical Diversity**:  
  - Robyn’s lyrics showed higher diversity (0.154) than Cher’s (0.091).  
  - Cher’s Twitter bios mirrored the lower diversity (0.091), showing limited variation.  

- **Most Common Emojis**:  
  - ❤️ 🌈 ✨ were dominant across both artists’ follower bios.  

- **Most Common Hashtags**:  
  - Political/social hashtags (#resist, #blm, #blacklivesmatter) were frequent for Cher.  
  - Music-related hashtags (#music, #edm) appeared in Robyn’s followers.  

- **Song Title Words**:  
  - Both artists had *love* as the most frequent title word.  

- **Song Lengths**:  
  - Cher’s songs tended to be longer on average, while Robyn’s were shorter but with greater lexical variety.  

---

## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/AnahitShekikyan/ADS509-Assignment2.1-Lyrics-Description-EDA.git
   cd ADS509-Assignment2.1-Lyrics-Description-EDA




