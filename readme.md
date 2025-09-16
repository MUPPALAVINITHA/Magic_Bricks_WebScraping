## 🏠 Rental Property Market Analysis
This project analyzes rental housing data scraped from MagicBricks, one of India’s leading real estate platforms. The goal is to uncover rental trends across five major Indian cities and provide insights into affordability, demand concentration, and market dynamics.

## 🎯 Objective
To analyze MagicBricks rental property data from five cities (Hyderabad, Bangalore, Mumbai, Chennai, Pune) in order to:
- Identify rental trends
- Compare city-level markets
- Assess factors driving rent
- Highlight top localities for tenants, owners, and investors

## 📊 Dataset Information
- Source: MagicBricks (web scraping)
- Records Collected: 1,000 (200 per city)
- Final Dataset (after cleaning): 815 rows × 8 columns

## Attributes Extracted:
City, BHK, Location, Price, Area (sqft), Property Type, Furnishing, Property Facing

## 🛠️ Tools & Libraries Used
- Python
- BeautifulSoup, Requests → Web scraping
- Pandas → Data cleaning & manipulation
- Regular Expressions (re) → Preprocessing numeric data
- Matplotlib, Seaborn → Visualization

## 🔄 Process / Workflow
Data Collection: Scraped 200 rental listings per city from MagicBricks.

Data Cleaning:
- Standardized location names
- Converted Price & Area → numeric values
- Filled missing values using mode
- Removed duplicates and unrealistic entries (e.g., BHK > 4, extreme outliers)

Data Storage: Final dataset saved as CSV for analysis.

## Exploratory Data Analysis: 
Conducted univariate, bivariate, and multivariate analysis.

## Univariate Analysis 
### Rental Price Distribution Across Cities
##### Key Insights: 
Mumbai has the highest average rent. 

Pune has the lowest average rent. 

Shows city-wise affordability of rental housing. 

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/620e404b-99c6-4ce1-bdbf-d6c2ced1ab14" />

### BHK vs Average Rent 
##### Key Insights: 
Average rent rises with number of BHKs. 

Higher BHKs → Higher rental cost. 

Helps renters & owners compare costs by BHK size. 

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/b2c74259-c0c9-4758-a0af-b04984860f95" />

### City-wise Furnishing Availability 
##### Key Insights: 
City-wise furnishing distribution.

Pune: More Furnished & Unfurnished. 

Bangalore: More Semi-Furnished. 

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/0d6fbe6f-3511-4ec3-9ea7-7539ba236980" />

### Property Type Market Share
##### Key Insights:
Flats dominate rental listings. 

Multiple property types available for rent. 

Reveals most common rental options. 

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/4b3645e7-a031-46ad-ab46-fe8abf677645" />

### Direction-wise Property Distribution 
##### Key Insights:
East-facing properties dominate the market. 

North & West have moderate availability. 

South-West & similar directions show very low supply. 

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/e4f32fb7-42d4-417a-acdd-1258585fba17" />

## Bivariate and Multivariate Analysis 
### Property Area vs Price Colored by BHK
##### Key Insights: 
Larger areas → Higher prices. 

Higher BHKs fall in higher price & area ranges. 

Color coding shows BHK-wise distribution clearly. 

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/17450b98-5773-4ec9-8b1c-0dc87634d920" />

## Top 5 Localities per City Based on Rent 
##### Key Insights: 
Ranks the costliest localities city-wise. 

Simplifies rental comparison within cities. 

Highlights prime areas with highest rents. 

<img width="1300" height="300" alt="image" src="https://github.com/user-attachments/assets/4495103e-3b83-4a17-a1c5-08c4fdd6751d" />

### Heatmap: Property Count by City and BHK 
##### Key Insights: 
2BHK & 3BHK dominate. 

Bangalore/Hyderabad: More 3BHK. 

Pune & Mumbai: More 2BHK. 

<img width="600" height="350" alt="image" src="https://github.com/user-attachments/assets/234386e2-e514-4ea8-8223-37b3be6851ff" />

### City-wise Rent Distribution by Locality 
##### Key Insights:
Shows top localities by total rent per city.

Larger blocks = higher rental contribution.

Identifies high-demand rental hotspots.

Useful for comparing rent concentration across cities.

<img width="845" height="79" alt="image" src="https://github.com/user-attachments/assets/b99f73f2-917e-4d3b-aa25-2ae86e957947" />
<img width="917" height="300" alt="image" src="https://github.com/user-attachments/assets/abf9447e-a304-4f2a-806a-73674047ba68" />

### Average Rent Comparison by Property Type 
##### Key Insights: Key Insights:  
Apartments lead with 31.1% of average rent share.  

Flats follow at 26.0%, also priced high.

Villas contribute 25.4% as premium options.

Houses have the lowest share (17.5%).

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/2e318747-1721-4398-8f6a-6ee3f9895fd6" />

### Heatmap: Average Rent by City, BHK and Furnishing 
##### Key Insights: 
3BHK & 4BHK command the highest rents, especially when furnished. 

Mumbai tops with premium rents (up to ₹1.45L+). 

Pune & Hyderabad remain budget-friendly (1BHK/2BHK). 

Bangalore & Chennai show mid-range trends. 

<img width="1459" height="652" alt="image" src="https://github.com/user-attachments/assets/ef749a82-4b32-4ff8-a1a6-6234b65a6057" />

### Conclusion 
The end-to-end EDA on rental property data provided valuable insights into how rents vary across cities, property types, and configurations. Through univariate, bivariate, and multivariate analysis, the study uncovered the key drivers of rent and highlighted affordability patterns, demand concentration, and overall market dynamics. 
Mumbai shows the highest rentals, while Pune & Hyderabad are more affordable. 

3BHK & 4BHK furnished units command premium rents. 

Area, furnishing, and facing direction are major rent drivers. 

Flats & apartments dominate the rental market. 

Locality-level insights highlight city-wise rental hotspots. 
