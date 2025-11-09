# Project X 
Group members: Y, Z

This repository contains the materials for **Project X**.  
- Presentation Slides: see [`slides/`](./slides/) folder  
- Notebooks: see [`notebooks/`](./notebooks/) folder
- Data: when you access correct data, place it in [`data/`](./data/) folder
- Results: the folder [`results/`](./result/) contains our figures and tables.
  
---
- Read more about this project on Medium: <Medium_Article_link>
---

## 📑 Project Outline


---
## 🚀 Environment Setup

Before starting, please **fork this repository** and create a fresh Python virtual environment.  
All required libraries are listed in `requirements.txt`.

> ⚠️ If you encounter errors during `pip install`, try removing the version pinning for the failing package(s) in `requirements.txt`.  
> On Apple M1/M2 systems you may also need to install additional system packages (the “M1 shizzle”).

---

### macOS / Linux (bash/zsh)

```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate

# Upgrade pip and install dependencies
pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (PowerShell)
```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
.venv\Scripts\Activate.ps1

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (Git Bash)
```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/Scripts/activate

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

You’re now ready to run the session notebooks!

Deactivate the environment when you’re done:
```bash
deactivate
```
## 🧠 Reflection — Phrase Diversity (n-gram TTR)
### 1. Which results matched your reading intuition?
Yes — the results matched expectations.
**_War and Peace_** had a slightly lower **TTR (phrase diversity)** compared to **_Anna Karenina_**.
This makes sense because *War and Peace* is a longer narrative with recurring military and philosophical language, while *Anna Karenina* focuses more on personal and emotional scenes, leading to greater phrase variety.

### 2. What surprised you?
It was surprising that the **difference between the two books was not very large**.
Even though *War and Peace* is much longer, Tolstoy’s phrasing remained rich and varied.
This shows that Tolstoy maintained a consistent and sophisticated writing style across different works.

### 3. If you toggled preprocessing (stopwords on/off), what changed?
When **stopwords were removed**, the **TTR increased slightly**.
This happens because very common words like *“of the”*, *“in the”*, and *“and the”* appear often and lower diversity.
Removing them makes the text seem more diverse by focusing on less frequent, more meaningful words.

### 4. Compare across the two works: are the patterns stable?
Yes — the **patterns are stable** across both novels:
- Both show similar **bigram vs trigram** relationships.
- The **TTR drops** from bigrams to trigrams, since longer phrases are more repetitive.
- *Anna Karenina* consistently shows a slightly **higher TTR**, reflecting more expressive and emotional variation compared to the more epic and repetitive style of *War and Peace*.

### 🧩 Summary Insight
Tolstoy’s language is consistently rich in both novels.
However, the **context and focus of each story** — epic versus intimate — shape their phrase diversity.
These results confirm that quantitative linguistic measures like TTR can meaningfully reflect an author’s literary style.
