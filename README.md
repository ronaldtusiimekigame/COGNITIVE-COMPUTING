# Personalized Educational Recommender
**A Cognitive Computing Approach for Ugandan Students**

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.28+-red.svg)](https://streamlit.io/)
[![License](https://img.shields.io/badge/License-Academic-green.svg)](LICENSE)

## Project Overview

This project implements a cognitive educational recommender system that helps Ugandan students find personalized learning resources. The system demonstrates four core cognitive pillars: **Understand**, **Reason**, **Learn**, and **Interact**.

**Scenario:** A Year 3 computing student at Uganda Christian University needs help understanding quantum computing and its relevance to Ugandan contexts (e.g., energy grid optimization).

**Course:** DSC3112 Cognitive Computing  
**Institution:** Uganda Christian University  
**Program:** Bachelor of Science in Data Science & Analytics

---

## Key Features

- **Semantic Understanding:** TF-IDF-based NLP for natural language query interpretation
- **Knowledge Graph Reasoning:** Multi-entity graph connecting courses, skills, universities, and topics with interactive visualization
- **Personalized Recommendations:** Query-aware course suggestions with dynamic relevance explanations
- **Uganda Context:** Automatically generates context-specific applications for Ugandan development challenges
- **Explainable AI:** Transparent reasoning showing why each course was recommended with similarity scores
- **Professional Interface:** Clean, organized Streamlit web application with neutral color scheme
- **Advanced Filtering:** Filter by difficulty, rating, and topic clusters
- **Course Explorer:** Browse and search all courses with detailed information
- **Performance Monitoring:** Real-time tracking of query processing times and system metrics
- **Query History:** Track your search history with export capabilities
- **Cognitive Demo:** Interactive demonstration of the four cognitive pillars

---

## Performance Metrics

- **Precision@5:** 0.72 (72% of recommendations are relevant)
- **Recall@5:** 0.68
- **Mean Reciprocal Rank (MRR):** 0.81
- **Response Time:** <1.2 seconds
- **Baseline Improvement:** 24% precision improvement over keyword search

---

## System Architecture

```
User Query
    ↓
[Understand] NLP + TF-IDF Vectorization
    ↓
[Reason] Knowledge Graph + Cosine Similarity Ranking
    ↓
[Interact] Dynamic Explanation Generation
    ↓
Personalized Recommendations with Uganda Context
    ↓
[Learn] Feedback Collection
```

---

## Repository Structure

```
COGNITIVE CO/
├── app.py                          # Streamlit web application
├── requirements.txt                 # Python dependencies
├── Coursera.csv                    # Raw dataset (3,424 courses)
├── notebooks/
│   └── PartB.ipynb                 # Implementation notebook (Tasks B1-B3)
├── artifacts/                      # Generated artifacts
│   ├── clean_courses.parquet       # Cleaned dataset
│   ├── tfidf_vectorizer.joblib     # Trained TF-IDF vectorizer
│   ├── tfidf_matrix.npz           # Course embeddings
│   └── knowledge_graph.html        # Interactive knowledge graph
├── docs/                           # Documentation
│   ├── PartA.md                    # Problem analysis & system design
│   ├── PartC_Evaluation_Report.md  # System evaluation
│   ├── PartC_Ethics_Impact_Analysis.md  # Ethics & impact analysis
│   ├── Final_Project_Report.md     # Comprehensive final report
│   └── Presentation_Outline.md    # Presentation structure
├── src/                            # Source code modules (if any)
└── README.md                       # This file
```

---

## Quick Start

### Prerequisites

- Python 3.8 or higher
- pip package manager

### Installation

1. **Clone or download this repository:**
   ```bash
   cd "COGNITIVE CO"
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Generate artifacts (if not already present):**
   - Run `notebooks/PartB.ipynb` to generate cleaned dataset and models
   - Or use pre-generated artifacts in `artifacts/` folder

4. **Launch the Streamlit application:**
   ```bash
   streamlit run app.py
   ```

5. **Open your browser:**
   - The app will automatically open at `http://localhost:8501`
   - If not, navigate to the URL shown in the terminal

---

## Usage

### Running the Application

1. **Start the app:**
   ```bash
   streamlit run app.py
   ```

2. **Navigate the interface:**
   - **Recommender Studio:** Main interface for entering queries and getting recommendations
   - **Knowledge Graph Explorer:** Interactive visualization of course relationships
   - **Insights & History:** Dataset statistics and query history
   - **Course Explorer:** Browse and search all available courses
   - **Cognitive Demo:** Learn about the four cognitive pillars

3. **Enter a query:**
   - Use the text area in Recommender Studio
   - Example: "Explain the basics of quantum computing and show me how it could be relevant for solving problems in Uganda"
   - The system accepts any natural language query about learning needs

4. **View recommendations:**
   - Top 5 courses are displayed with:
     - Course name and university
     - Difficulty level and rating
     - Similarity score (match quality)
     - Clickable Coursera URL
     - Dynamic relevance explanation
     - Uganda-specific context

5. **Use advanced features:**
   - Apply filters (difficulty, rating, topic) for refined results
   - View recommendation insights (topic coverage, skills analysis)
   - Explore the knowledge graph to understand relationships
   - Browse all courses in the Course Explorer

6. **Provide feedback:**
   - Click "Helpful" or "Not Helpful" to provide feedback
   - Feedback is tracked and displayed in statistics

### Example Queries

- "Explain quantum computing basics and relevance to Uganda's energy grid"
- "I need data analysis skills for agricultural supply chain optimization"
- "Business strategy courses for tech startups in Kampala"
- "Machine learning for healthcare in East Africa"
- "Python programming for beginners"
- "Creative storytelling techniques for STEM outreach"

---

## Technical Details

### Technologies Used

- **Python 3.8+:** Core programming language
- **Streamlit:** Web application framework
- **scikit-learn:** TF-IDF vectorization, cosine similarity
- **pandas:** Data manipulation and analysis
- **NetworkX:** Knowledge graph construction
- **PyVis:** Interactive graph visualization
- **NumPy, SciPy:** Numerical computations

### Cognitive Components

1. **Understanding Engine:**
   - TF-IDF vectorization with n-grams (1-2)
   - Query preprocessing (tokenization, stopword removal)
   - Intent detection (quantum mention, Uganda context)

2. **Reasoning Engine:**
   - Knowledge graph with 120+ courses, 80+ skills
   - Cosine similarity ranking
   - Multi-entity relationship modeling

3. **Learning Component:**
   - Feedback collection (Helpful/Not Helpful)
   - Ready for future integration into ranking algorithm

4. **Interaction Layer:**
   - Streamlit web interface
   - Progressive spinners showing cognitive processing
   - Dynamic explanation generation

---

## Evaluation

See `docs/PartC_Evaluation_Report.md` for comprehensive evaluation including:
- Quantitative metrics (precision, recall, MRR)
- Baseline comparison (TF-IDF vs. keyword search)
- Error analysis
- Recommendations for improvement

---

## Ethical Considerations

See `docs/PartC_Ethics_Impact_Analysis.md` for detailed analysis of:
- Data bias and fairness
- Privacy considerations
- Contextual appropriateness for Ugandan users
- Mitigation strategies

**Key Findings:**
- Dataset bias toward Western content (mitigation: data augmentation)
- English-only content (mitigation: multilingual support planned)
- Privacy by design (minimal data collection)

---

## Documentation

### User Documentation
- **README.md:** Project overview and quick start (this file)
- **USER_MANUAL.md:** Comprehensive user guide with step-by-step instructions
- **docs/UI_FEATURES.md:** Detailed interface documentation

### Academic Documentation
- **docs/PartA.md:** Problem Analysis & System Design (30 marks)
- **docs/Final_Project_Report.md:** Comprehensive final project report
- **docs/PartC_Evaluation_Report.md:** System evaluation report (10 marks)
- **docs/PartC_Ethics_Impact_Analysis.md:** Ethics & impact analysis (5 marks)
- **docs/Presentation_Outline.md:** Presentation structure and talking points
- **docs/DOCUMENTATION_INDEX.md:** Complete documentation index

### Implementation
- **notebooks/PartB.ipynb:** Implementation notebook (Tasks B1-B3, 50 marks)
- **app.py:** Streamlit web application (Task B3)

---

## Academic Context

**Course:** DSC3112 Cognitive Computing  
**Institution:** Uganda Christian University  
**Program:** Bachelor of Science in Data Science & Analytics  
**Year:** 3, Semester 1  
**Examination Type:** 100% Project-Based Exam  
**Duration:** Two Weeks (December 2025)

**Milestones:**
1. ✅ System Blueprint & Data Pipeline
2. ✅ Understanding Engine
3. ✅ Interactive Prototype
4. ✅ Evaluation & Ethical Review
5. ✅ Final Documentation & Presentation

---

## Future Work

### Short-Term (1-3 months)
- User profiling system
- Query expansion with synonyms
- Feedback integration into ranking

### Medium-Term (3-6 months)
- Deep learning models (BERT, Sentence-BERT)
- Enhanced knowledge graph with prerequisites
- Conversational interface

### Long-Term (6-12 months)
- Adaptive learning system
- Bias mitigation framework
- UCU Moodle integration

---

## Contributing

This is an academic project for DSC3112 Cognitive Computing. For questions or suggestions:
- Review the documentation in `docs/`
- Check the implementation notebook `notebooks/PartB.ipynb`
- Refer to the evaluation report for performance details

---

## License

This project is created for academic purposes as part of the DSC3112 Cognitive Computing course at Uganda Christian University.

---

## Author

**Student Name:** [Your Full Name]  
**Registration Number:** [Your Reg Number]  
**Institution:** Uganda Christian University  
**Course:** DSC3112 Cognitive Computing  
**Date:** December 2025

---

## Acknowledgments

- Uganda Christian University Faculty of Engineering, Design and Technology
- Department of Computing and Technology
- Coursera for open educational content dataset
- Open-source community for excellent tools (Streamlit, scikit-learn, NetworkX, PyVis)

---

## Contact

For questions about this project, please refer to the documentation or contact through UCU academic channels.

---

**Last Updated:** December 2025  
**Version:** 1.0

