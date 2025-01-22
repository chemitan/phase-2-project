# Movie Analysis Project

## Overview
This project aims to identify what types of movies perform best in terms of profitability, how production budgets relate to revenue, and which strategies can enhance international market performance. By analyzing multiple datasets (including IMDb data, budget information, and box office revenues), we uncover actionable insights for movie studios and stakeholders looking to optimize their production strategies.

## Motivation & Business Understanding
Despite significant investments, some high-budget films underperform due to misaligned strategies, while moderate-budget films sometimes achieve unexpected success. This project addresses:

- Which types of movies are most profitable?
- How do production budgets correlate with domestic and worldwide revenues?
- What strategies can maximize performance in international markets?

**Stakeholders** include movie studios, producers, and investors seeking to make data-driven decisions about future productions.

## Data Understanding
This project uses data from six primary sources:

1. **tn.movie_budgets.csv.gz**  
   - **Key Features:** `production_budget`, `domestic_gross`, `worldwide_gross`.

2. **bom.movie_gross.csv.gz**  
   - **Key Features:** `domestic_gross`, `foreign_gross`, `year`.

3. **rt.movie_info.tsv.gz**  
   - **Key Features:** `synopsis`, `genre`, `box_office`.

4. **rt.reviews.tsv.gz**  
   - **Key Features:** `review`, `rating`, `critic`, `publisher`.

5. **im.db**  
   - **Key Features:** `genres`, `averagerating`, `primary_title`.

6. **tmdb.movies.csv**  
   - **Key Features:** `popularity`, `vote_average`, `genre_ids`.

All datasets were cleaned (e.g., removing `$` signs, converting strings to numeric, handling missing values) to ensure consistency. When necessary, files were merged (e.g., matching movies by title or identifiers) for comprehensive analysis.

## Methodology / Approach
1. **Data Loading & Cleaning**  
   - Imported CSV/TSV files and connected to the IMDb SQLite database (`im.db`).  
   - Performed data type conversions and handled missing values.

2. **Exploratory Data Analysis (EDA)**  
   - Generated scatter plots to analyze budgets vs. profitability/revenues.  
   - Created bar charts for genre profitability, popular genres by ratings, studio performance, and top crew members.

3. **Insights & Interpretations**  
   - Investigated how budget allocations affect domestic vs. worldwide revenue.  
   - Identified high-performing genres and key contributors (directors, writers, studios).

4. **Recommendations**  
   - Provided data-driven advice on budgets, genres, crew collaboration, and marketing to maximize profitability.

## Analysis & Visualizations
- **Scatter Plots**: Production Budget vs. Profitability, Budget vs. Revenue (Domestic and Worldwide).  
- **Bar Charts**: Genre profitability, top-performing directors/writers, studios, etc.  
- **Additional Plots**: Depict popular movies by vote count, ratings, and more.

## Results & Key Insights
1. **High-Budget Films** generally yield higher worldwide revenue but may underperform without strong execution.  
2. **Genre & Franchise Power**: Family, Fantasy, and franchise-based films have significant global appeal and profitability.  
3. **Crew & Studio Influence**: Established directors, writers, and studios consistently boost profitability through effective storytelling, production quality, and marketing.

## Recommendations
1. **Invest in High-Performing Genres & Franchises**: Comedy, Family, Fantasy, Sci-Fi, etc.  
2. **Collaborate with Proven Talent**: Directors and writers with track records of success.  
3. **Balance Budget & Strategy**: Support large investments with thorough market research and global marketing.

## How to Run the Project
1. **Clone or Download** this repository.
2. **Install Requirements** (e.g., `pandas`, `matplotlib`, `seaborn`, `sqlite3`).
3. **Open the Notebook** in Jupyter (or compatible environment).
4. **Run the Notebook Cells** to replicate the analysis and generate the visualizations.

## Project Structure
├── data │ ├── tn.movie_budgets.csv.gz │ ├── bom.movie_gross.csv.gz │ ├── rt.movie_info.tsv.gz │ ├── rt.reviews.tsv.gz │ ├── tmdb.movies.csv │ └── im.db ├── notebooks │ └── Movie_Analysis.ipynb ├── presentation.pdf ├── README.md └── requirements.txt


## Author / Contact
**Your Name**  
- **Email**: abumorgan@gmail.com  
- **LinkedIn**: https://www.linkedin.com/in/morgan-a-140948124/

Feel free to reach out for questions, feedback, or collaboration!
