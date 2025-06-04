# 🦠 COVID Cases Analysis

This project investigates how COVID-19 case and death rates across U.S. states correlate with socioeconomic and political factors such as poverty rates, median income, educational attainment, and 2020 presidential election results.

It was originally created as a final project for my SI 206 (Data-Oriented Programming) class at the University of Michigan. Although I haven’t modified the code beyond what was submitted, I wanted to present it here as a complete, standalone showcase of what I built—highlighting my ability to work with APIs, web scraping, databases, and data visualization in Python.

## 📊 Overview

We collect and integrate data from multiple sources—public APIs and web scraping—and analyze it using SQLite and Python. The project stores this data in a relational database, performs joins across tables, and produces visualizations to explore meaningful trends.


## 🔍 Data Sources

- **COVID-19 API**: State-level case, death, population, and testing data  
- **U.S. Census Bureau API**: Poverty population, median income, education levels  
- **Wikipedia**: Scraped data on 2020 U.S. presidential election results by state  

## 📁 Features

- ✅ Fetches and stores live data from COVID and Census APIs  
- ✅ Scrapes election data from Wikipedia using BeautifulSoup  
- ✅ Creates a normalized SQLite database with multiple joined tables  
- ✅ Plots graphs using `matplotlib` to show correlations such as:
  - COVID case rate vs. political affiliation
  - Death rate by party
  - Median income vs. case rate
  - Bachelor's degree rate vs. case rate  
- ✅ Exports results and stats to a human-readable `results.txt` file  
- ✅ Saves all visualizations to a `/findings` directory

## 📦 Tech Stack

- **Python 3**
- `requests`, `json`, `sqlite3`, `matplotlib`, `BeautifulSoup`
- SQLite for local relational data storage
- Structured using modular functions and single `main()` runner

## 🖥️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/COVID-cases-analysis.git
   cd COVID-cases-analysis
   
## ⚠️ Notes

    Only the first 25 states are inserted into the database per execution to limit redundancy and ensure performance.

    You’ll need an active internet connection for the APIs and Wikipedia scraping to work.

    Ensure your Census API key is inserted into the API_KEY variable at the top of main.py.
