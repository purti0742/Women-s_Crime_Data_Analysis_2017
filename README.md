# Women's Crime Data Analysis Across Indian Cities

## Project Overview
This project analyzes crimes against women across multiple Indian cities using statistical methods and data visualization. The analysis focuses on identifying patterns, multi-victim incidents, and crime distribution across different crime categories under Indian Penal Code (IPC) and State-specific laws.

## Objective
- Clean and standardize large-scale crime dataset (164+ columns)
- Identify multi-victim crime incidents through ratio analysis
- Detect statistical outliers in crime patterns
- Visualize crime distribution to identify high-risk cities and crime trends

## Dataset
- **Source**: Indian crime statistics data (crimes against women)
- **Format**: CSV
- **Columns**: 164 features covering:
  - Murder with Rape/Gang Rape (IPC)
  - Dowry Deaths (IPC Section 304B)
  - Human Trafficking (IPC Section 370 & 370A)
  - Cyber Crimes under IT Act (Women-centric violations)
  - State-specific laws (SLL)
- **Metrics**: Incidence (I), Victims (V), Rate (R) for each crime category

## Key Findings
✓ Standardized 30+ verbose column names into concise, analyzable identifiers  
✓ Identified cities with multi-victim crime incidents (victim-to-incident ratio > 1.0)  
✓ Detected statistical outliers in Dowry Death cases using Interquartile Range (IQR) method  
✓ Ranked top 5 cities by cyber crime volume  
✓ Created comparative visualizations across 5 crime categories  

## Analysis Performed
1. **Data Cleaning**: Removed null values, standardized column names, handled zero-division errors
2. **Ratio Analysis**: Computed victim-to-incident ratios for 8 crime metrics
3. **Statistical Analysis**: IQR-based outlier detection, descriptive statistics
4. **Visualization**: Bar plots (city-wise comparison), Box plots (distribution analysis)
5. **Exploratory Data Analysis**: Statistical summaries and trend identification

## Technical Stack
- **Language**: Python 3.x
- **Libraries**:
  - Pandas (data manipulation & analysis)
  - Matplotlib (data visualization)
  - Seaborn (statistical visualization)
- **Environment**: Jupyter Notebook

## Project Structure
```
crime-analysis/
│
├── crime.ipynb                 # Main analysis notebook
├── data_123.csv                # Crime dataset
├── README.md                   # This file
├── requirements.txt            # Python dependencies
└── RESUME_FINDINGS.md          # Resume-ready summary
```

## How to Run

### Prerequisites
- Python 3.7+
- pip (Python package manager)

### Installation
1. Clone the repository:
```bash
git clone <repository-url>
cd crime-analysis
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Open the Jupyter Notebook:
```bash
jupyter notebook crime.ipynb
```

4. Run cells sequentially to reproduce the analysis

## Key Code Sections

### Data Preprocessing
- Column renaming and standardization
- Missing value analysis and handling
- Feature selection (consolidation from 164 to 26 columns)

### Ratio Calculations
- Victim-to-incident ratios for each crime category
- Error handling for zero-division scenarios

### Statistical Analysis
- Quartile calculations (Q1, Q3) for outlier detection
- Descriptive statistics (mean, median, std dev)
- IQR-based anomaly detection

### Visualizations
- Bar plots showing victim-to-incident ratios by city
- Box plots displaying ratio distributions across crime types
- City rankings by cyber crime volume

## Key Insights

### Multi-Victim Incidents
Identified cities where single incidents involved multiple victims (ratio > 1.0):
- Particularly prevalent in Human Trafficking cases
- Notable in Cyber Crime categories (blackmailing, defamation)

### Outlier Cities
Dowry Death cases showed statistical outliers using IQR method, indicating unusual patterns requiring further investigation.

### Cyber Crime Trends
Top 5 cities ranked by cyber crime incidents, with distinct patterns in:
- Publishing/transmitting sexually explicit material
- Blackmailing, defamation, morphing, fake profiles

## Skills Demonstrated
- Data cleaning and preprocessing
- Statistical analysis and outlier detection
- Data visualization and storytelling
- Exploratory Data Analysis (EDA)
- Python programming (Pandas, Matplotlib, Seaborn)

## Future Enhancements
- Time-series analysis to track crime trends over years
- Correlation analysis between crime categories
- Predictive modeling for crime hotspots
- Interactive dashboards using Plotly/Dash
- Geographical mapping of crime data

## Author
[Your Name]

## License
This project is for educational purposes.

## References
- Indian Penal Code (IPC) sections referenced
- State-specific crime law classifications
