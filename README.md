🏅 Summer Olympic Medals Analysis (1976–2008)
This repository contains a cleaned dataset and analysis of Summer Olympic medal winners from 1976 to 2008. It enables exploration of medal counts by country, sport, gender, and year to uncover performance trends and historical patterns.

📁 Files in this Repository
Summer-Olympic-medals-1976-to-2008.csv – Dataset containing Olympic medal records.

(Optional) Olympics_analysis.ipynb – Jupyter Notebook with analysis and visualizations.

(Optional) README.md – This documentation.

📊 Dataset Description
Each row represents a medal awarded in a Summer Olympic event between 1976 and 2008.

Column Name	Description
City	Host city of the Olympic Games
Year	Year of the Games
Sport	Broad sport category (e.g., Athletics)
Discipline	Specific sport discipline (e.g., Track)
Event	Event name (e.g., 100m Men’s Final)
Athlete	Name of the athlete
Gender	Male or Female
Country_Code	IOC country code (e.g., USA, CHN)
Country	Full country name
Event_gender	Gender category of the event (M or W)
Medal	Type of medal (Gold, Silver, Bronze)

🧪 Sample Analysis Code
python
Copy code
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

df = pd.read_csv("Summer-Olympic-medals-1976-to-2008.csv")

# Top 10 countries by total medals
top_countries = df['Country'].value_counts().head(10)

sns.barplot(x=top_countries.values, y=top_countries.index, palette="viridis")
plt.title("Top 10 Countries by Total Medals (1976–2008)")
plt.xlabel("Number of Medals")
plt.show()
📈 Insights You Can Explore
🏆 Top countries by total medals or gold medals

👩‍🦰 Gender participation trends over the years

🏃‍♂️ Most successful sports and disciplines

🧍‍♂️ Most decorated athletes

🌍 Medal distribution by continent or region

📅 Time series analysis of medal growth

🔧 Tools Used
Python – Programming language

Pandas – Data manipulation

Seaborn / Matplotlib – Data visualization

(Optional) Power BI or Excel for dashboard views

📌 Example Visualizations
Bar plots for top countries

Pie charts for gender share

Line graphs for medal growth

Heatmaps for country-sport performance

📝 How to Use
Clone this repository:

bash
Copy code
git clone https://github.com/Deepak2gr/Summer-Olympic-medals-1976-to-2008.git
Install required packages:

bash
Copy code
pip install pandas seaborn matplotlib
Run the Jupyter Notebook or your own Python script to explore and visualize.

📜 License
This project is open source. You are free to use, modify, and share the dataset and analysis with proper citation.

👤 Author
Deepak Kumar
📧 LinkedIn
💼 Aspiring Data Analyst | Python • Excel • Power BI • SQL

