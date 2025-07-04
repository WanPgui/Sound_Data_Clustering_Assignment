Sound Data Clustering Assignment
# Sound Data Clustering Assignment

##  Project Title
**Clustering and Dimensionality Reduction of an Unlabeled Sound Dataset**

---

Link to HMM for capstone idea: https://docs.google.com/document/d/1FpUufeMmGvHyqO7sCoXHo5uoxaXeZBv4nucwwvv4DjE/edit?usp=sharing

---


##  Description

This project applies **clustering techniques** to an unlabeled sound dataset to explore the use of **dimensionality reduction** and evaluate different clustering algorithms. The goal is to uncover potential groupings within sound recordings based solely on extracted features, while analyzing the interpretability, accuracy, and real-world applicability of the clustering results.

The dataset consists of 3000 unlabeled audio files provided in a `.zip` format and extracted to a working directory. The project was completed in a Google Colab Jupyter notebook, supported with visualizations, markdown explanations, and a final write-up discussing practical applications of Hidden Markov Models in a real-world use case.

---

##  Objectives

- Extract Mel Spectrogram features from audio signals.
- Attempt raw feature visualizations and discuss the necessity of dimensionality reduction.
- Apply **PCA** and **t-SNE** for dimensionality reduction and compare their effectiveness.
- Cluster the data using **K-Means** and **DBSCAN**.
- Optimize hyperparameters (e.g., number of clusters for K-Means).
- Evaluate clustering results using metrics and visualizations.
- Reflect on algorithm performance, visual separation, and interpretability.
- Describe how **Hidden Markov Models (HMMs)** could be used in the related capstone project.

---

##  Dataset

- **Source:** Provided zip file `unlabelled_sounds.zip`
- **Contents:** 3000 unlabeled `.wav` audio files
- **Preprocessing:** Mel Spectrogram features extracted using `librosa`

---

##  Technologies Used

- **Python**
- **Google Colab**
- **Librosa** – for audio feature extraction
- **NumPy, Pandas** – for data manipulation
- **Scikit-learn** – for PCA, KMeans, DBSCAN, evaluation metrics
- **Matplotlib, Seaborn** – for data visualization
- **FPDF** – to generate a structured PDF explanation of HMMs

---

##  Project Workflow

### 1. **Data Loading & Feature Extraction**
- Loaded `.wav` files from Google Drive after extracting the zip file.
- Extracted **Mel Spectrogram** features with fixed shape per file.
- Stored features as a NumPy array.

### 2. **Initial Visualization (Without Dimensionality Reduction)**
- Attempted scatter and pair plots using raw feature dimensions.
- Discussed the limitations and interpretability challenges.
- Justified the need for dimensionality reduction.

### 3. **Dimensionality Reduction**
- Applied **PCA** and **t-SNE** to reduce features to 3 dimensions.
- Compared the two methods using 3D scatter plots.
- Evaluated which technique offered clearer cluster separation.

### 4. **Clustering Algorithms**
- Applied **K-Means Clustering**:
  - Used the **Elbow Method** and **Silhouette Score** to determine optimal `k`.
  - Visualized resulting clusters in reduced dimensional space.
- Applied **DBSCAN**:
  - Tuned `eps` and `min_samples` parameters.
  - Compared DBSCAN clustering quality with K-Means.

### 5. **Evaluation Metrics**
- Compared **Inertia**, **Silhouette Score**, and **Davies-Bouldin Index** for both algorithms.
- Discussed visual interpretability and compactness of clusters.

### 6. **Final Analysis (Markdown Summary)**
- Justified dimensionality reduction based on clearer cluster separation.
- Explained algorithm performance differences.
- Related results to practical clustering problems.

### 7. **Part 2: Capstone Use Case for HMM**
- Explained how a **Hidden Markov Model** can track hidden health states using observable data like meals, symptoms, and vitals.
- Identified known and unknown values in the HMM setup.
- Generated a PDF titled `HMM_Capstone_Explanation.pdf` with a human-readable summary of the approach.

---

##  Results

- **PCA** offered cleaner cluster separation than raw data, but **t-SNE** provided more visually distinct clusters.
- **K-Means** worked well after tuning `k`, while **DBSCAN** required careful parameter tweaking and was sensitive to density variations.
- Dimensionality reduction significantly improved clustering performance and interpretability.

---

##  Capstone Integration

**Capstone Title:**
“Machine Learning-Powered Mobile Nutrition Assistant for Chronic Disease Management in Nairobi’s Low-Income Communities”

- Used an HMM to detect user health states based on dietary and biometric logs.
- Aimed at improving chronic disease monitoring and early intervention through probabilistic modeling.

PDF summary is included in the repo as:  
 `HMM_Capstone_Explanation.pdf`

---

##  Repository Contents
 sound_clustering/
├── unlabelled_sounds/ # Extracted audio files
├── Formative_1_sound_clustering_assignment.ipynb # Main Jupyter Notebook
├── HMM_Capstone_Explanation.pdf # Final HMM summary PDF
├── README.md # This file


---

##  How to Run the Project

1. Upload `unlabelled_sounds.zip` to your Google Drive.
2. Mount Google Drive in Colab.
3. Run the notebook step-by-step:
   - Extract zip
   - Extract Mel Spectrograms
   - Apply PCA/t-SNE
   - Perform clustering
   - Evaluate and interpret results

---

##  Submission Instructions

- **Submission 1 (Attempt 1):** Zip the entire folder including the notebook, PDF, and data (excluding large audio files if needed).
- **Submission 2 (Attempt 2):** Push everything to a GitHub repository and share the link.

---

##  Author

**Peris Wangui**  
BSc in Software Engineering  
ALU 
