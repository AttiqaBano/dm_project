**Story Evolution Tracking & News Cycle Pattern Analysis**
**Project Overview**

This project analyzes 213,740 news articles from two major Pakistani English newspapers (Dawn & Daily Times, 2015–2023) to study story evolution and news cycle patterns. It tracks narrative, sentiment, entity, and framing evolution across 1,247 distinct stories and quantifies news lifecycle dynamics including lifespan, intensity, decay, and resurgence.

**Features & Methodology**

**Data Preprocessing:** Cleaning, category mapping, feature engineering, TF-IDF vectorization, temporal standardization.

Story Identification: Cosine similarity (threshold 0.6) and 7-day temporal window clustering.

Evolution Tracking: Phase-based keyword shifts, sentiment trajectories (VADER), entity tracking (SpaCy), framing analysis.

News Cycle Analysis: Lifespan classification, intensity patterns, decay rate calculation, resurgence detection.

Machine Learning: Sentiment classification (Logistic Regression: 99.79% accuracy), topic modeling (LDA), clustering (KMeans).

**Key Findings**

72.4% of stories exhibit significant narrative evolution; 44.9% become more negative over time.

Political stories have the longest lifespan (12.7 days) and highest entity turnover, while sports stories show rapid decay (half-life 2.1 days).

Early coverage patterns can predict story duration with 67.3% accuracy; resurgence occurs in 15% of stories.

**Applications**

Editorial decision support for resource allocation.

Automated story tracking and clustering in large news archives.

Audience engagement optimization and misinformation detection.

**Limitations & Future Work**

Fixed similarity threshold and 7-day window may miss loosely connected or slow-burning stories.

VADER sentiment may misclassify culturally specific expressions; entity recognition accuracy can vary for local names.

Future work: real-time implementation, multi-modal analysis, Urdu-language comparison, causal modeling, and audience behavior integration.

**Technical Details**

Programming: Python 3.8+ (Pandas, NumPy, Scikit-learn)

NLP Libraries: SpaCy, NLTK, VADER, TF-IDF Vectorizer

Computing: Google Colab with GPU acceleration

Dataset: Pakistani news corpus (2015–2023)
