# Game-Sales-Dashboard
This project examines global video game sales to uncover insights into trends across genres, platforms, publishers, and regions. The analysis utilizes a Tableau dashboard, Python-based exploratory analysis, and a processed dataset to provide actionable insights for stakeholders in the gaming industry.

---

## Step-by-Step Explanation

### 1. Raw Data
**Contents:**  
- **Source:** The raw dataset `data/game_sales_data.csv` contains 16,598 records with the following key attributes:  
  - **Rank:** Game rank based on total global sales.  
  - **Name:** Game title.  
  - **Platform:** Platform on which the game was released (e.g., PS3, Wii).  
  - **Year:** Year of release.  
  - **Genre:** Game genre (e.g., Action, Sports).  
  - **Publisher:** Game publisher.  
  - **NA_Sales, EU_Sales, JP_Sales, Other_Sales, Global_Sales:** Sales data by region and total sales globally (in millions of units).  
- **Issues:**  Missing values in `Year` and `Publisher`, and mixed data types in `Year`.  

---

### 2. Data Processing
**Objective:**  
Clean the dataset for accurate analysis.

**Steps:**  
- Removed rows with missing values in `Year` and `Publisher`.  
- Converted `Year` to integer for consistency.  
- Renamed columns for clarity (e.g., `NA_Sales` → `North_America_Sales`).  

**Output:**  
Processed dataset saved as `data/processed_game_sales_data.csv`.

---

### 3. Exploratory Analysis
We used a Jupyter notebook `notebooks/exploratory_analysis.ipynb` to explore and analyze the processed data:  

- **Summary Statistics:** Calculated descriptive stats for key attributes.  
- **Top 10 Games:** Identified the highest-selling games globally.  
- **Genre Sales Distribution:** Visualized sales distribution across game genres using a boxplot.  
- **Yearly Trends:** Analyzed global sales over time to identify peaks and trends.  

**Key Insights:**  
- Action and Sports genres dominate sales.  
- Global sales peaked during certain years, reflecting significant releases or platform milestones.  

---

### 4. Tableau Visualizations
#### Selected Visualizations:
1. **Top 10 Games by Global Sales** (`visuals/top_games_sales.png`):  
   - **Interpretation:** Identifies the most successful games, with *Wii Sports* leading global sales at 82.74 million units.  
   - **Insight:** Highlights the dominance of Nintendo titles in the top-selling list.

2. **Yearly Sales Trends by Genre** (`visuals/genre_sales_trends.png`):  
   - **Interpretation:** Combined line and area chart showing annual sales trends, categorized by genre.  
   - **Insight:** Action and Sports genres consistently lead sales, while Racing shows peaks during specific years.

3. **Sales by Platform** (`visuals/platform_sales_distribution.png`):  
   - **Interpretation:** Bubble chart displaying sales performance across platforms.  
   - **Insight:** PS3, Xbox 360, and Wii are top platforms, reflecting the technological advancements and market dominance during their era.

4. **Top Publishers by Sales** (`visuals/publisher_sales.png`):  
   - **Interpretation:** Tree map visualizing publishers' contributions to global sales.  
   - **Insight:** Nintendo and Electronic Arts are market leaders, emphasizing their global influence.

**Additional Insights:**  
1. Regional Preferences: Sales vary significantly by region, indicating opportunities for targeted marketing.  
2. Platform Trends: Peaks in sales align with major platform launches or breakthroughs.  

---

### 5. Key Insights
- **Top Games:** *Wii Sports*, *Grand Theft Auto V*, and *Mario Kart Wii* dominate global sales.  
- **Genre Insights:** Action and Sports genres show consistent popularity, while Racing spikes in specific years.  
- **Regional Variations:** Preferences differ, with Nintendo excelling in Japan and North America.  
- **Platform Trends:** PS3, Xbox 360, and Wii are the most impactful platforms.  

---

### 6. How to Use
1. **Clone the repository:**
   ```bash
   git clone https://github.com/srideepthi-vootla/Game-Sales-Dashboard.git

2. **Data and Analysis:**
- View raw and processed datasets in `data/`.  
- Explore data trends in `notebooks/exploratory_analysis.ipynb`.  

3. **Visualization:**
- Open the Tableau workbook in `dashboard/game_sales_dashboard.twb`.  
- Review key visuals in the `visuals/` folder.  

---

### 7. Tools and Technologies
- **Python:** Data cleaning and exploratory analysis.  
- **Tableau:** Interactive dashboards and visualizations.  
- **Seaborn/Matplotlib:** Visualization in Python.  

---

### Future Scope
- Predict future trends using machine learning models.  
- Perform regional demographic analysis for market targeting.  
- Extend analysis to include user reviews and ratings. 

---
  
### Contributors
- **Sri Deepthi Vootla**  
- **Jayakishan Minnekanti**  
