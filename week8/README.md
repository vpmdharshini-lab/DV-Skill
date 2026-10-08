# Students Performance Visualization

## Project Overview
This project analyzes student performance data using Python and visualizes the results through various charts and graphs. The analysis focuses on student scores in Mathematics, Reading, and Writing, along with demographic factors such as gender, parental education level, lunch type, and test preparation course.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Dataset
The project uses a preprocessed dataset:

`studentperformance_preprocessed.csv`

The dataset contains:
- Math Score
- Reading Score
- Writing Score
- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch Type
- Test Preparation Course

## Features

### 1. Data Exploration
- Display first and last records
- Dataset information
- Statistical summary
- Column inspection
- Missing value analysis
- Dataset dimensions

### 2. Demographic Analysis
- Gender distribution
- Parental education categories
- Lunch type categories
- Test preparation course categories

### 3. Visualizations

#### Grouped Bar Chart
Shows average Mathematics, Reading, and Writing scores based on parental education level.

#### Bar Plot
Displays average percentage scores by parental education level and lunch type.

#### Box Plot
Compares score distributions for students who completed and did not complete the test preparation course.

#### Pair Plot
Shows pairwise relationships among Mathematics, Reading, and Writing scores.

#### Correlation Heatmap
Visualizes correlations between the three exam scores.

## Installation

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn
```

## How to Run

1. Download the dataset:
   `studentperformance_preprocessed.csv`

2. Place the dataset in the appropriate directory.

3. Run the Python script:

```bash
python students_performance_visualization.py
```

## Expected Output
The program generates:
- Grouped Bar Chart
- Average Score Bar Plot
- Box Plot
- Pair Plot
- Correlation Heatmap

These visualizations help understand factors affecting student performance and identify relationships between exam scores.

## Learning Outcomes
- Data preprocessing and exploration
- Statistical analysis using Pandas
- Data visualization using Matplotlib and Seaborn
- Correlation analysis
- Educational performance analysis


## License
This project is developed for academic and educational purposes.
