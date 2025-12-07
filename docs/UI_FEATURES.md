# User Interface Features Documentation
**Personalized Educational Recommender System**

**Version:** 1.0  
**Date:** December 2025

---

## Overview

The Personalized Educational Recommender features a professional, clean interface designed for academic presentation. The interface uses a neutral color scheme (grays, whites, subtle blues) and is organized into five main functional areas accessible via tabs.

---

## Interface Design Principles

### Color Scheme
- **Primary Colors:** Grays (#2c3e50, #34495e, #95a5a6)
- **Backgrounds:** Whites and light grays (#f8f9fa, #ecf0f1, #ffffff)
- **Accents:** Subtle blue (#3498db) for information boxes
- **Charts:** Grayscale and neutral color scales
- **No Emojis:** Professional text-only interface

### Layout Organization
- **Header Section:** Title and subtitle with gradient background
- **Performance Metrics:** System performance dashboard
- **Dataset Overview:** Statistics and visualizations
- **Main Content:** Tabbed interface for different functions
- **Sidebar:** System information and quick statistics

---

## Main Interface Components

### 1. Header Section

**Location:** Top of page

**Components:**
- Main title: "Cognitive Computing – Personalized Educational Recommender Agent"
- Subtitle: "Scenario 3: Personalized Educational Recommender for Ugandan Students"
- Professional gradient background (dark gray)

### 2. System Performance Metrics

**Location:** Below header

**Metrics Displayed:**
- Precision@5: 0.72 (+24% vs baseline)
- Recall@5: 0.68 (+31% improvement)
- Average Response: 0.9s (Real-time)
- Courses Indexed: Total count

**Purpose:** Quick overview of system performance

### 3. Dataset Overview

**Location:** Below performance metrics

**Components:**
- Four statistics: Quantum Courses, Uganda Context, Average Rating, Unique Skills
- Two bar charts: Topic Distribution, Difficulty Distribution

**Purpose:** Provide context about the dataset

### 4. Sidebar

**Location:** Left side of interface

**Sections:**
- **System Information:** Cognitive pillars mapping
- **System Performance:** Average response time, total queries, reset button
- **Dataset Statistics:** Total courses, quantum courses, Uganda context

**Purpose:** Always-visible system information and quick stats

---

## Tabbed Interface

### Tab 1: Recommender Studio

**Primary Function:** Main interface for getting course recommendations

**Components:**

1. **Sample Query Buttons**
   - Five pre-filled query suggestions
   - Click to populate query field

2. **Query Input Area**
   - Large text area for entering study needs
   - Placeholder with example
   - Height: 120px

3. **Advanced Filters & Preferences** (Expandable)
   - Difficulty Levels: Multi-select dropdown
   - Minimum Rating: Slider (0.0 to 5.0)
   - Topic Focus: Multi-select dropdown

4. **Get Personalized Recommendations Button**
   - Primary button, full width
   - Triggers the cognitive processing cycle

5. **Recommendation Display**
   - Success message with course count
   - Performance metrics (average similarity, top similarity, processing time)
   - Numbered course cards (1-5) with:
     - Course name and match score
     - University, difficulty, rating, topic
     - Course URL link
     - Relevance explanation (info box)
     - Uganda context (info box)

6. **Recommendation Insights** (Tabbed)
   - **Topic Coverage:** Bar chart of topic distribution
   - **Skills Analysis:** Bar chart and table of top skills
   - **Similarity Distribution:** Plotly bar chart of similarity scores

7. **Feedback Section**
   - "Helpful" and "Not Helpful" buttons
   - Feedback quality progress bar
   - Statistics display

**Key Features:**
- Real-time processing with progress indicators
- Similarity scores for transparency
- Dynamic explanations
- Comprehensive insights

---

### Tab 2: Knowledge Graph Explorer

**Primary Function:** Interactive visualization of course relationships

**Components:**

1. **Search and Filter Controls**
   - Search input for courses or skills
   - Topic filter dropdown
   - Difficulty filter dropdown

2. **Interactive Graph Display**
   - PyVis network graph (700px height)
   - Clickable and draggable nodes
   - Color-coded node types

3. **Graph Statistics**
   - Four metrics: Courses, Skills, Universities, Connections

4. **Graph Interpretation Guide** (Expandable)
   - Node type explanations
   - Interpretation guidelines

**Key Features:**
- Interactive exploration
- Search highlighting
- Filtering capabilities
- Educational guide

---

### Tab 3: Insights & History Dashboard

**Primary Function:** Dataset statistics and query history

**Components:**

1. **Dataset Statistics** (Two rows of metrics)
   - Row 1: Total Courses, Uganda Context, Quantum Courses, Universities
   - Row 2: Average Rating, Unique Skills, Difficulty Levels, Topic Clusters

2. **Visualizations**
   - Topic Distribution (bar chart)
   - Difficulty Distribution (bar chart)
   - Rating Distribution (histogram using Plotly)
   - Top 10 Universities (bar chart)

3. **Query History**
   - Clear history button
   - Export to CSV button
   - Expandable entries showing:
     - Query text
     - Timestamp
     - Courses found count
     - Results dataframe

**Key Features:**
- Comprehensive statistics
- Multiple visualizations
- History tracking
- Export functionality

---

### Tab 4: Course Explorer

**Primary Function:** Browse and search all available courses

**Components:**

1. **Search and Filter Controls**
   - Full-text search input
   - Topic filter dropdown
   - Difficulty filter dropdown

2. **Results Display**
   - Courses found metric
   - Pagination selector (10 courses per page)
   - Expandable course cards with:
     - Course name and university
     - Metadata (difficulty, rating, topic)
     - Skills count
     - Quantum/Uganda context indicators
     - Course description (truncated)
     - Course URL link

3. **Course Comparison Tool**
   - Two course selectors
   - Side-by-side comparison display
   - Metrics comparison

**Key Features:**
- Full dataset access
- Advanced search
- Detailed course information
- Comparison functionality

---

### Tab 5: Cognitive Demo

**Primary Function:** Educational demonstration of cognitive computing principles

**Components:**

1. **Four Pillar Tabs:**
   - **Understand:** Query processing demonstration
   - **Reason:** Algorithm explanation and visualization
   - **Learn:** Feedback statistics and future enhancements
   - **Interact:** Interaction flow and live demo

2. **Interactive Elements:**
   - Query processing demo input
   - Live demo button with progress indicators
   - Algorithm formulas (LaTeX)
   - Flow diagrams

**Key Features:**
- Educational content
- Interactive demonstrations
- Algorithm transparency
- Live examples

---

## User Experience Features

### Real-Time Feedback
- Progress spinners during processing
- Success/error messages
- Performance metrics display
- Feedback statistics

### Responsive Design
- Wide layout for better visibility
- Organized columns and sections
- Expandable sections for advanced features
- Tabbed interface for organization

### Professional Styling
- Clean CSS with neutral colors
- Consistent spacing and padding
- Subtle shadows and borders
- Clear typography hierarchy

### Accessibility
- Clear labels and descriptions
- Logical flow and organization
- Helpful tooltips and guides
- Error messages and warnings

---

## Technical Implementation

### Technologies Used
- **Streamlit:** Web application framework
- **Plotly:** Interactive visualizations
- **PyVis:** Knowledge graph visualization
- **Custom CSS:** Professional styling

### Performance Optimizations
- Cached resource loading
- Efficient data processing
- Real-time performance tracking
- Optimized visualizations

---

## Future Enhancements

Potential improvements for future versions:
- User profiles and preferences
- Saved recommendation lists
- Email export functionality
- Mobile-responsive design
- Dark mode option
- Accessibility improvements (screen reader support)

---

**Documentation Prepared By:** [Your Name]  
**Last Updated:** December 2025


