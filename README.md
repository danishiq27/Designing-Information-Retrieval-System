# News Articles Information Retrieval System

A comprehensive information retrieval system for business and sports news articles, implementing multiple retrieval methods including Boolean, BM25, TF-IDF, and a hybrid approach.

## 🚀 Quick Start (Google Colab - Recommended)

### Option 1: Open in Colab (Easiest)
1. **Open the notebook**: [Open in Google Colab](your_colab_link_here)
2. **Upload dataset**: When prompted, upload the `Articles.csv` file
3. **Run all cells**: Click Runtime → Run all
4. **View results**: The system will automatically run comprehensive evaluation

### Option 2: Manual Setup in Colab
```python
# 1. Upload the notebook to Google Colab
# 2. Run these commands in order:

!git clone https://github.com/danishiq27/Designing-Information-Retrieval-System.git
%cd your-repo-name

# 3. Upload Articles.csv when prompted
# 4. Run all cells sequentially

📁 Project Structure
├── information_retrieval_system.ipynb  # Main Colab notebook
├── Articles.csv                        # Dataset (2692 news articles)
├── README.md                          # This file
└── requirements.txt                   # Python dependencies


🛠️ Local Installation (Alternative)
If you prefer to run locally:
Prerequisites
Python 3.8+
4GB RAM minimum

Installation Steps
# Clone repository
git clone https://github.com/danishiq27/Designing-Information-Retrieval-System.git
cd your-repo-name

# Install dependencies
pip install -r requirements.txt

# Run the system
python ir_system.py

Dependencies
rank-bm25==0.2.1
nltk==3.8.1
scikit-learn==1.3.0
pandas==2.0.3
chardet==5.2.0
matplotlib==3.7.1

📊 Dataset Information
Total Documents: 2,692 news articles
Business Articles: 1,284
Sports Articles: 1,408
Columns: Article, Date, Heading, NewsType

🔍 Features Implemented
Retrieval Methods
Boolean Retrieval - Exact term matching with AND logic

BM25 - Probabilistic relevance scoring
TF-IDF - Vector space model with cosine similarity
Hybrid - BM25 recall + TF-IDF precision ranking

Advanced Features
Phrase search using quotes ("stock market")
News type filtering (business/sports)
Comprehensive evaluation framework
Performance comparison charts

📈 Expected Output
When you run the notebook, you'll see:

System Statistics - Document count, vocabulary size, etc.
Method Comparison - All 4 methods tested on 10 queries
Performance Analysis - Speed and result count comparisons
Advanced Features Demo - Phrase search and filtering examples

⏱️ Performance Metrics
Based on our evaluation:

Boolean: Fastest (0.0014s avg) but no ranking
BM25: Good balance (0.0055s avg) with probabilistic scoring
TF-IDF: Moderate speed (0.0031s avg) with vector similarity
Hybrid: Most sophisticated (0.0083s avg) with best ranking quality

🐛 Troubleshooting
Common Issues
NLTK Download Errors: The code includes fallback tokenization
Encoding Issues: Automatic encoding detection handles most cases
Memory Limits: For large collections, reduce max_features in TF-IDF

Getting Help
If you encounter issues:
Check that all dependencies are installed
Ensure Articles.csv is in the correct directory
Run cells in order (don't skip any)


👨‍💻 Author
Danish iqbal
GitHub: danishiq27
Project: Information Retrieval and Text Mining Assignment

📄 License
This project is for academic purposes as part of Information Retrieval and Text Mining assignment.

**Save this as `README.md`** (not .txt) in your GitHub repository. GitHub automatically renders Markdown files with proper formatting, making it look professional and easy to read.
If you specifically need a .txt file instead, let me know and I'll provide a plain text version!
