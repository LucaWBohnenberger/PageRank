# 📊 PageRank Algorithm Implementation

This project was developed as part of **Harvard's Introduction to Artificial Intelligence (CS50's AI)** course. It implements the **PageRank algorithm**, which measures the importance of web pages based on their links. Using a **Markov Chains** model, the program simulates the behavior of a user browsing the web to compute the probability distribution of the most relevant pages. 📊🔗

---

## ✨ Features

- 📈 Computes **PageRank scores** for a set of interlinked pages.
- 🔄 Supports both **iterative** and **Markov Chain (random surfer)** approaches.
- 📂 Reads web structures from **HTML files**, parsing links automatically.
- 💻 Includes a command-line interface for experimentation.

---

## 📂 Datasets

The repository includes sample datasets consisting of **HTML pages** with links between them. The structure is automatically processed to extract:

1. **📁 corpus/**: Contains multiple HTML pages representing a small-scale web structure. The program extracts hyperlinks from these pages.

2. **🔗 Link Graph**: Represents connections between pages, forming a directed graph used for PageRank calculation.

---

## ⚙️ How It Works

1. **📝 Input**:
   - The program loads a set of interlinked HTML pages from the corpus.

2. **💡 Processing**:
   - **Iterative Algorithm**: Starts with equal rank distribution and updates values iteratively until convergence.
   - **Random Surfer Model**: Uses a stochastic approach where a virtual user randomly follows links to approximate rankings.

3. **📤 Output**:
   - Displays the **PageRank scores** for each page after convergence.

---

## 🎬 Example Run

**Command:**
```bash
python pagerank.py corpus0
```

**Output:**
```
PageRank Results for corpus0:
page1.html: 0.324
page2.html: 0.243
page3.html: 0.216
page4.html: 0.217
```

---

## 💡 Key Learnings

This project provided insights into:
- 🌍 **Graph Representation**: Modeling the web as a directed graph.
- 🔄 **Iterative Convergence**: Implementing and optimizing iterative methods for rank propagation.
- 🎲 **Markov Chains**: Understanding probability distributions in the random surfer model.
- 🛠️ **Web Crawling & Parsing**: Extracting hyperlink structures from HTML files.

---

## 🚀 Usage

1. **📥 Clone the repository**:
   ```bash
   git clone https://github.com/LucaWBohnenberger/PageRank
   ```

2. **📂 Navigate to the project directory**:
   ```bash
   cd PageRank
   ```

3. **▶️ Run the program**:
   ```bash
   python pagerank.py (name of folder with pages, e.g.: corpus0)
   ```

