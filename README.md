# League-of-Legends Bigdata Analysis with Spark

## Project Overview
This project analyzes data from the Riot API using Apache Spark to extract insights from over 180,000 matches across different ranked tiers (high elo and low elo). The analysis includes champion statistics, item synergies, win rates, and other key metrics to understand gameplay patterns.

## Technologies Used
- **Apache Spark** (PySpark)
- **Google Colab**
- **Python** (Riot Watcher API, Pandas, JSON Processing)
- **Tableau** (For data visualization)

## Data Collection
The dataset was collected from the Riot API using multiple Riot accounts to speed up the data retrieval process. The matches were gathered from several servers: **EUW, NA, KR**.

### Data Format
- The raw match data is stored in **JSON** files.
- Processed data is converted to **CSV** files for further analysis and visualization.
- The dataset includes:
  - Match details
  - Champion picks and win rates
  - Item selections and synergies
  - Champion duos and bans

## Analysis Process
1. **Data Collection**
   - Used Riot Watcher API to fetch match data.
   - Stored data in JSON format.
2. **Data Cleaning & Organization**
   - Structured data into relevant categories.
   - Removed inconsistencies and prepared the dataset.
3. **Analysis with PySpark**
   - Implemented custom functions to extract meaningful statistics.
   - Calculated win rates, pick rates, item synergies, and champion performance metrics.
4. **Data Visualization**
   - Processed results into CSV format.
   - Created graphs and charts using Tableau.

## Key Insights
### Champions (High Elo vs. Low Elo)
- Most picked champion: **Jhin (High Elo)**, **Ezreal (Low Elo)**
- Highest win rate: **Aurelion Sol (55.7%) in High Elo**, **Sona (54.4%) in Low Elo**
- Most banned champion: **Zed (40k+ bans)**
- Best champion synergy: **Lucian & Nami (High Elo)**, **Jhin & Lux (Low Elo)**

### Items
- Most picked item: **Ionian Boots of Lucidity (High Elo)**, **Berserker's Greaves (Low Elo)**
- Highest win rate item: **Mejai’s Soulstealer (80%) in both tiers**

### Champion Matchups
- Most played matchup: **Jhin vs. Jinx (1969 matches)**
- Win rate: **Jhin (50.23%) vs. Jinx (49.77%)**
- Best & worst matchups calculated for each champion.

## File Structure
```
📂 League-of-Legends-big-data-analysis-with-Spark
├── 📂 Analysis
│   ├── SparkAnalysis.ipynb (Main analysis script)
│
├── 📂 Output
│   ├── 📂 Results
│   ├── 📂 Graphs
│   ├── Other Outputs
├── Technical Report.pdf
├── Business Report.pdf
└── README.md (This file)
```

## Future Improvements
- Expand dataset to include more matches.
- Improve item and champion recommendation algorithm.
- Implement real-time data updates.

---
**Contributions and feedback are welcome!** Feel free to open issues or submit pull requests.
