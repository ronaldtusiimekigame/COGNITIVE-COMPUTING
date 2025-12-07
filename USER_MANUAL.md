# User Manual
**Personalized Educational Recommender System**

**Version:** 1.0  
**Date:** December 2025

---

## Table of Contents

1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Using the Application](#using-the-application)
4. [Understanding Recommendations](#understanding-recommendations)
5. [Tips for Best Results](#tips-for-best-results)
6. [Troubleshooting](#troubleshooting)
7. [FAQ](#faq)

---

## 1. Introduction

### What is This System?

The Personalized Educational Recommender is a cognitive computing system that helps you find relevant online courses based on your learning needs. It understands your queries, reasons over a knowledge base of 3,400+ courses, and provides personalized recommendations with explanations.

### Who Is This For?

- **Primary Users:** UCU BSc Data Science & Analytics students
- **Use Case:** Finding relevant courses for exam preparation, skill development, or topic exploration
- **Example:** "I need to understand quantum computing and how it applies to Uganda's energy sector"

### Key Features

- **Natural Language Queries:** Ask questions in plain English
- **Personalized Recommendations:** Top 5 courses matched to your needs with similarity scores
- **Explainable Results:** See why each course was recommended with dynamic relevance explanations
- **Uganda Context:** Understand how courses apply to local challenges with context-specific applications
- **Fast Response:** Results in less than 2 seconds
- **Advanced Filtering:** Filter by difficulty, rating, and topic
- **Knowledge Graph:** Interactive visualization of course relationships
- **Course Explorer:** Browse and search all available courses
- **Performance Monitoring:** Real-time system performance metrics
- **Query History:** Track your searches with export capabilities

---

## 2. Getting Started

### System Requirements

- **Web Browser:** Chrome, Firefox, Safari, or Edge (latest versions)
- **Internet Connection:** Required for accessing course links
- **No Installation Needed:** Runs in your web browser

### Accessing the Application

1. **Start the Application:**
   - If running locally: `streamlit run app.py`
   - The app will open automatically in your browser
   - URL: `http://localhost:8501`

2. **First Time Use:**
   - No account creation required
   - No login needed
   - Start querying immediately

---

## 3. Using the Application

### Step 1: Enter Your Query

**Location:** Large text area at the top of the page

**What to Enter:**
- Describe what you want to learn
- Include context about your goals
- Mention any specific applications (e.g., "for Uganda's agriculture sector")

**Example Queries:**
- Good: "Explain quantum computing basics and show relevance to Uganda's energy grid"
- Good: "I need data analysis skills for agricultural supply chain optimization"
- Good: "Business strategy courses for tech startups in Kampala"
- Too vague: "help me learn"
- Too specific: "course ID 12345"

**Tips:**
- Be specific about topics you're interested in
- Mention your learning goals or applications
- Include context (e.g., "for beginners" or "advanced level")

### Step 2: Apply Filters (Optional)

**Advanced Filters:**
- **Difficulty Levels:** Select preferred difficulty (Beginner, Intermediate, Advanced, Mixed)
- **Minimum Rating:** Set a minimum course rating (0.0 to 5.0)
- **Topic Focus:** Filter by topic clusters (Quantum Computing, Data & AI, Business, Creative, Other)

**Location:** Click "Advanced Filters & Preferences" expander in Recommender Studio

### Step 3: Click "Get Personalized Recommendations"

**What Happens:**
1. **Understanding your query...** (0.3 seconds)
   - System processes your natural language query
   - Extracts key topics and intent
   - Preprocesses text for semantic matching

2. **Reasoning over knowledge base...** (0.3-0.6 seconds)
   - Searches through 3,400+ courses
   - Computes cosine similarity scores
   - Applies filters if specified
   - Ranks courses by relevance

3. **Generating recommendations...** (0.3 seconds)
   - Generates personalized explanations
   - Creates Uganda-specific context
   - Formats results for display

**Total Time:** Less than 1.5 seconds (typically 0.9 seconds)

### Step 3: Review Recommendations

**What You'll See:**

For each of the top 5 courses:

1. **Course Name** (bold heading)
   - The full title of the course
   - Numbered ranking (1-5)

2. **Match Score** (metric display)
   - Similarity score showing how well the course matches your query
   - Higher scores indicate better relevance

3. **University**
   - Institution offering the course

4. **Metadata** (three columns)
   - **Difficulty:** Beginner, Intermediate, Advanced, Mixed
   - **Rating:** X.X/5 (if available)
   - **Topic:** Topic cluster classification

5. **Course Link**
   - Clickable link to the course on Coursera
   - Opens in a new tab

6. **Relevance Explanation** (info box)
   - Why this course matches your query
   - Specific topics and skills covered
   - Generated dynamically based on course content and your query

7. **Uganda Context** (info box)
   - How the course applies to Ugandan challenges
   - Specific applications (e.g., agriculture, health, energy)
   - Local institution references when relevant

### Step 4: Review Recommendation Insights

**Location:** Below the recommendations

**Available Insights:**
- **Topic Coverage:** Bar chart showing topic distribution in recommendations
- **Skills Analysis:** Top skills represented in recommended courses
- **Similarity Distribution:** Visual comparison of similarity scores

**Additional Statistics:**
- Number of unique universities
- Average rating of recommendations
- Total unique skills covered
- Difficulty level diversity

### Step 5: Provide Feedback (Optional)

**Location:** Bottom of Recommender Studio tab

**Options:**
- **Helpful:** Click if recommendations were useful
- **Not Helpful:** Click if recommendations didn't meet your needs

**Feedback Tracking:**
- Feedback is collected and displayed in statistics
- Progress bar shows feedback quality percentage
- Counts are maintained across the session
- Future versions will use feedback to improve recommendations

---

## 4. Exploring Additional Features

### Knowledge Graph Explorer

**Purpose:** Visualize relationships between courses, skills, universities, and topics

**Features:**
- Interactive graph with clickable nodes
- Search functionality to highlight specific courses or skills
- Filters by topic and difficulty
- Graph statistics (courses, skills, universities, connections)
- Interpretation guide explaining node types

**How to Use:**
1. Navigate to "Knowledge Graph Explorer" tab
2. Use search to find specific courses or skills
3. Apply filters to focus on specific topics or difficulty levels
4. Click and drag nodes to explore connections
5. Review graph statistics and interpretation guide

### Insights & History Dashboard

**Purpose:** View dataset statistics and track your query history

**Features:**
- Comprehensive dataset statistics (total courses, Uganda context, quantum courses)
- Visualizations (topic distribution, difficulty distribution, rating histogram)
- Top universities chart
- Query history with timestamps
- Export history as CSV

**How to Use:**
1. Navigate to "Insights & History" tab
2. Review dataset overview statistics
3. Explore visualizations
4. View your query history
5. Export history if needed

### Course Explorer

**Purpose:** Browse and search all available courses

**Features:**
- Full-text search across course names, universities, and topics
- Filter by topic and difficulty
- Paginated results (10 courses per page)
- Detailed course information in expandable cards
- Course comparison tool

**How to Use:**
1. Navigate to "Course Explorer" tab
2. Enter search terms or apply filters
3. Browse results page by page
4. Expand course cards for detailed information
5. Use comparison tool to compare two courses side-by-side

### Cognitive Demo

**Purpose:** Learn about the four cognitive pillars

**Features:**
- Detailed explanations of Understand, Reason, Learn, and Interact pillars
- Interactive query processing demo
- Algorithm visualization
- Feedback statistics
- Live demonstration of cognitive cycle

**How to Use:**
1. Navigate to "Cognitive Demo" tab
2. Explore each pillar tab
3. Try the query processing demo
4. Review algorithm details
5. Run the live demo to see the cognitive cycle in action

## 5. Understanding Recommendations

### How Recommendations Are Generated

The system uses **semantic similarity** to match your query with courses:

1. **Your Query** → Converted to numerical representation (TF-IDF)
2. **Course Descriptions** → Also converted to numerical representation
3. **Similarity Calculation** → Measures how similar your query is to each course
4. **Ranking** → Courses sorted by similarity score
5. **Top 5 Selection** → Best matches displayed

**Why This Matters:**
- Understands meaning, not just keywords
- Handles synonyms (e.g., "ML" = "machine learning")
- Considers context and intent

### Understanding Relevance Explanations

**Dynamic Relevance:**
- Generated specifically for each course
- Based on actual course content (description, skills)
- Matches your query terms to course topics

**Example:**
- Query: "quantum computing for energy"
- Relevance: "This course directly addresses your interest in quantum computing by teaching Quantum Mechanics, Qiskit, and covers quantum computing fundamentals with practical examples."

### Understanding Uganda Context

**Purpose:** Connect global knowledge to local applications

**How It Works:**
- Analyzes course skills and topics
- Maps to Ugandan development challenges
- References local institutions and sectors

**Examples:**
- Data Analysis → "crop yield prediction for Ugandan farmers"
- Health Courses → "disease surveillance for Village Health Teams"
- Business Courses → "startups at Innovation Village, Kampala"
- Energy Courses → "energy grid optimization for Uganda's power networks"

---

## 6. Tips for Best Results

### Writing Effective Queries

✅ **DO:**
- Be specific about topics: "machine learning for healthcare"
- Include your goals: "I want to learn Python for data analysis"
- Mention applications: "quantum computing for energy optimization"
- Add context: "business strategy for tech startups in Uganda"

❌ **DON'T:**
- Use single words: "python" (too broad)
- Be too vague: "help me learn" (not specific enough)
- Use course codes: "DSC3112" (system doesn't know course codes)
- Ask yes/no questions: "Is quantum computing hard?"

### Getting Diverse Recommendations

**If you want variety:**
- Use broader queries: "data science" instead of "Python pandas tutorial"
- System automatically provides diversity across topics and skills

**If you want specific focus:**
- Use detailed queries: "quantum computing basics with Qiskit for beginners"
- System will prioritize exact matches

### Understanding Course Information

**Difficulty Levels:**
- **Beginner:** No prior knowledge required
- **Intermediate:** Some background knowledge helpful
- **Advanced:** Requires significant prior experience
- **Mixed:** Multiple difficulty levels

**Ratings:**
- Based on Coursera student reviews
- Scale: 1.0 to 5.0
- Higher ratings indicate better student satisfaction

**Universities:**
- Various institutions worldwide
- Includes top universities (Stanford, MIT, etc.)
- Note: Limited African universities in current dataset

---

## 7. Troubleshooting

### Problem: No Recommendations Appear

**Possible Causes:**
- Query too vague or unclear
- No courses match your query
- Technical error

**Solutions:**
1. Try rephrasing your query with more specific terms
2. Check if your query contains relevant keywords
3. Refresh the page and try again
4. Contact support if problem persists

### Problem: Recommendations Seem Irrelevant

**Possible Causes:**
- Query ambiguity
- Vocabulary mismatch between query and course descriptions

**Solutions:**
1. Add more context to your query
2. Use synonyms or alternative terms
3. Try breaking complex queries into simpler parts
4. Provide feedback ("Not Helpful") to help improve system

### Problem: Course Links Don't Work

**Possible Causes:**
- Course may have been removed from Coursera
- URL format issue
- Network connectivity problem

**Solutions:**
1. Check your internet connection
2. Try copying the URL and pasting in browser
3. Search for the course name directly on Coursera
4. Note: Some courses may require Coursera subscription

### Problem: Slow Response Times

**Possible Causes:**
- Large query processing
- System load
- Network latency

**Solutions:**
1. Normal response time: 1-2 seconds (be patient)
2. If >5 seconds, refresh and try again
3. Check your internet connection speed

---

## 8. FAQ

### Q: What are the different tabs in the interface?

**A:** The interface has five main tabs:
- **Recommender Studio:** Main interface for queries and recommendations
- **Knowledge Graph Explorer:** Interactive visualization of course relationships
- **Insights & History:** Dataset statistics and query history
- **Course Explorer:** Browse and search all courses
- **Cognitive Demo:** Learn about the cognitive computing pillars

### Q: What is the similarity score?

**A:** The similarity score (0.0 to 1.0) indicates how well a course matches your query. Higher scores mean better relevance. Scores are computed using cosine similarity between your query and course descriptions.

### Q: Can I save my recommendations?

**A:** Yes! The system automatically saves your query history. You can:
- View your history in the "Insights & History" tab
- Export your query history as CSV
- See up to 5 most recent queries with full details

### Q: How accurate are the recommendations?

**A:** Based on evaluation:
- 72% of top-5 recommendations are relevant (Precision@5: 0.72)
- 68% recall rate (Recall@5: 0.68)
- Mean Reciprocal Rank of 0.81
- System significantly outperforms simple keyword search (24% improvement)
- Recommendations improve with more specific queries

### Q: Can I filter by difficulty level or topic?

**A:** Currently, the system doesn't have explicit filters. However:
- You can include difficulty in your query: "beginner Python course"
- You can specify topics: "machine learning for healthcare"
- Future versions may include filter options

### Q: What filters can I apply?

**A:** You can filter recommendations by:
- **Difficulty Levels:** Beginner, Intermediate, Advanced, Mixed
- **Minimum Rating:** Set a threshold (0.0 to 5.0)
- **Topic Clusters:** Quantum Computing, Data & AI, Business, Creative, Other

Filters are applied in the "Advanced Filters & Preferences" section.

### Q: Is my query data stored?

**A:** Query history is stored in your browser session:
- Queries are saved locally in the session
- History includes query text, timestamp, and results
- You can clear history at any time
- History is not persisted after closing the browser
- Feedback is collected and displayed in statistics

See Privacy Policy in documentation for details.

### Q: Can I use this for other subjects besides computing?

**A:** Yes! The system works for any topic available in the Coursera dataset:
- Business, Finance, Strategy
- Data Science, AI, Machine Learning
- Design, Creative Arts
- Health, Education
- And more!

### Q: How do I provide feedback?

**A:** After viewing recommendations:
1. Scroll to the bottom of the page
2. Click "Helpful" or "Not Helpful"
3. Your feedback is logged (currently to terminal)
4. Future versions will use feedback to improve recommendations

### Q: Can I access this on mobile?

**A:** Yes! The Streamlit interface is mobile-responsive. However:
- Best experience on desktop/laptop
- Course links work on mobile browsers
- Some features may be optimized for larger screens

---

## Getting Help

### For Technical Issues:
- Check the Troubleshooting section above
- Review the README.md for technical details
- Check system requirements

### For Academic Questions:
- Refer to project documentation in `docs/` folder
- Review the Final Project Report
- Consult course instructor

### For Feature Requests:
- Feedback is welcome for future improvements
- Note limitations in current version
- See Future Work section in documentation

---

## Version History

**Version 1.0 (December 2025)**
- Initial release
- Basic recommendation functionality
- TF-IDF semantic retrieval
- Knowledge graph visualization
- Uganda context generation
- Feedback collection

---

**Manual Prepared By:** [Your Name]  
**Last Updated:** December 2025  
**For:** DSC3112 Cognitive Computing Project

