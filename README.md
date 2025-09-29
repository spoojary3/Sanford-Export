# Seafood Export Analysis

## Objective
Analyze seafood exports to identify:
- Right Market: Best growth/pricing countries
- Right Product: Most profitable species/products
- Right Price: Optimal pricing strategy by market

## Data Source
- Source files: Exports CSVs from Sanford loaded into s3 bucket
- Fiscal years: 2023-2024
- Data includes: Species, Product, Country, Volume, Value

## Methodology
1. **Data Extraction**
   - SQL scripts in `ETL.SQL`
2. **Data Transformation**
   - Cleaning
   - SQL scripts in `ETL.SQL`
3. **Data Loading**
   - Load into Power BI for visualization by connecting to Snowflake
     
4. **Have used star schema  for scalability and enhanced filtering and slicing**
   <img width="649" height="360" alt="image" src="https://github.com/user-attachments/assets/dd8462c3-d9b9-400b-8f17-ff15ac5efc8b" />


5. **Analysis and Key Findings**
   - MARKET POSITIONING: EXPORT GROWTH VS PRICE PER KG
     Shows export growth (%) vs price per kg by country.
     Countries like Vietnam, Denmark, Netherlands and Canada appear in favorable positions with higher growth and pricing.
     Bubble size  indicate export volume — larger bubbles suggest more significant markets.
   - Table to show growth/pricing across countries
     Vietnam and Denmark lead in combined growth and pricing potential.
   - PRICING_STRATEGY: PROFITABLE MARKET
      High volume and high price — ideal for profitability
   - Heatmaps for market profitability species and bar chart for product
      Mussels are the most valuable 
   - PBIX files in `pbix/SANFORD_EXPORT_ANALYSIS.PBIX`
- Have used star schema  for scalability and enhanced filtering and slicing

## Usage
1. Open PBIX files in Power BI Desktop
2. Explore visuals and findings


