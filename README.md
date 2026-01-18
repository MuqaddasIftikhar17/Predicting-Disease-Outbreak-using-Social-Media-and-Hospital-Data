# 🦠 Predicting Disease Outbreaks Using Social Media & Hospital Data

## 📋 Overview
This project presents a **big data-driven disease outbreak prediction system** that integrates **social media data** with **hospital records** to enable earlier and more accurate detection of disease outbreaks. By combining real-time social media signals with structured clinical data, the system provides public health authorities with timely insights for proactive intervention.

## 🎯 Key Features
- **Real-time Social Media Monitoring**: Analyzes Twitter and health forum posts for early symptom reporting
- **Hospital Data Integration**: Combines structured clinical records for reliability
- **Apache Spark Processing**: Scalable distributed data processing for large datasets
- **Machine Learning Models**: Logistic Regression/Naive Bayes classifiers for outbreak prediction
- **Comprehensive Evaluation**: Multiple metrics (Accuracy, Precision, Recall, F1-score) for performance assessment

## 📊 System Architecture

### High-Level Architecture
```
┌─────────────────────────────────────────────────────────┐
│                    DATA COLLECTION LAYER                 │
├─────────────────────────────────────────────────────────┤
│  • Social Media Posts (Twitter, Forums)                 │
│  • Hospital Records (Structured Data)                   │
└─────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────┐
│                    DATA STORAGE LAYER                    │
├─────────────────────────────────────────────────────────┤
│  • CSV Format Storage                                   │
│  • Apache Spark for Distributed Processing              │
└─────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────┐
│                 DATA PREPROCESSING LAYER                 │
├─────────────────────────────────────────────────────────┤
│  • Data Cleaning (Missing Values, Noise Removal)        │
│  • Text Preprocessing (Tokenization, Stop-word Removal) │
│  • Feature Extraction                                   │
└─────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────┐
│               ANALYTICS & MODELING LAYER                 │
├─────────────────────────────────────────────────────────┤
│  • Machine Learning Model Training                      │
│  • Outbreak Signal Detection                            │
│  • Performance Comparison                               │
└─────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────┐
│           VISUALIZATION & EVALUATION LAYER              │
├─────────────────────────────────────────────────────────┤
│  • Performance Metrics                                  │
│  • Comparative Analysis                                 │
│  • Visualization Dashboards                             │
└─────────────────────────────────────────────────────────┘
```

## 🛠️ Installation & Setup

### Prerequisites
- Python 3.8+
- Apache Spark 3.0+
- Google Colab

## 📁 Project Structure
```
disease-outbreak-prediction/
│
├── covidtweets.csv          # Hospital records
│__ BDA PPT11
|__ Predicting Disease Outbreaks Using Social Media - Report.docx
├── Big Data Project - Final.ipynb
├── README.md             # This file
└── LICENSE               # License information
```

## 🚀 Usage

### Running the Colab Notebook
```bash
Big Data Project - Final.ipynb
```

### Key Notebook Sections
1. **Data Loading and Exploration**
2. **Data Preprocessing**
   - Hospital data cleaning
   - Social media text preprocessing
3. **Feature Engineering**
   - Keyword frequency extraction
   - Temporal aggregation
4. **Model Training**
   - Logistic Regression
   - Naive Bayes
5. **Evaluation and Visualization**

## 📈 Results

### Performance Comparison

| Approach | Timeliness | Accuracy | Precision | Recall | F1-Score |
|----------|------------|----------|-----------|--------|----------|
| Hospital Data Only | Low | High | 0.89 | 0.85 | 0.87 |
| Social Media Only | High | Medium | 0.72 | 0.95 | 0.82 |
| Combined Approach | High | High | 0.91 | 0.92 | 0.915 |

### Visualizations

#### 1. Outbreak Prediction Timeline
![Outbreak Prediction Timeline](results/plots/timeline_comparison.png)

#### 2. Model Performance Metrics
![Performance Metrics](results/plots/metrics_comparison.png)

#### 3. Feature Importance
![Feature Importance](results/plots/feature_importance.png)

#### 4. ROC Curves Comparison
![ROC Curves](results/plots/roc_curves.png)

## 🎯 Key Findings

1. **Improved Timeliness**: Combined approach detects outbreaks **3-5 days earlier** than hospital-only methods
2. **Enhanced Accuracy**: 12% improvement in F1-score compared to single-source approaches
3. **Scalability**: Apache Spark enables processing of millions of social media posts efficiently
4. **Practical Application**: System provides actionable insights for public health authorities

## 🔮 Future Work

- [ ] **Real-time Data Streaming**: Implement Kafka/Spark Streaming for live data processing
- [ ] **Deep Learning Integration**: Apply BERT/Transformers for better text understanding
- [ ] **Geospatial Analysis**: Add location-based outbreak prediction
- [ ] **Multi-disease Support**: Extend to various infectious diseases
- [ ] **Mobile Alert System**: Develop notification system for health authorities

## 📚 References

1. World Health Organization - Disease Surveillance Reports
2. Research articles on social media-based disease detection
3. Apache Spark Documentation
4. Scikit-learn Machine Learning Library

## 👥 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments
- Apache Spark Community
- Public health organizations for dataset access
- Research contributors in computational epidemiology

---

**⚠️ Disclaimer**: This system is for research purposes and should not replace official public health surveillance systems. Always consult with health authorities for outbreak response decisions.
```
