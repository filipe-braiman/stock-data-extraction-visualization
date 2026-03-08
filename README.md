# Stock Data Extraction and Visualization

**Enhanced Adaptation of IBM Data Science Professional Certificate Project**

## Project Overview

This project is an enhanced adaptation of my "Python Project for Data Science" course completed to obtain my [IBM Data Science Professional Certificate on Coursera](https://coursera.org/share/839efad34c9080742b9d556d8c7d608b). The project demonstrates practical skills in financial data extraction and visualization by collecting and analyzing stock data for Tesla (TSLA) and GameStop (GME).

The project combines API data extraction with web scraping techniques to gather comprehensive financial data, then creates interactive visualizations to display stock performance and revenue trends.

## Project Objectives

* Extract real-time stock data using the yfinance API
* Scrape historical revenue data from financial websites using BeautifulSoup
* Create interactive visualizations combining stock price and revenue data
* Compare performance trends between technology and retail stocks
* Demonstrate end-to-end data extraction and visualization workflow

## Repository Structure

```
stock-data-extraction-visualization/
├── Stock_Data_Extraction+Visualization.ipynb  # Main Jupyter notebook with complete analysis
├── Datasets/                                   # Extracted data in CSV format
│   ├── tesla_stock_data.csv
│   ├── tesla_revenue.csv
│   ├── gamestop_stock_data.csv
│   ├── gamestop_revenue.csv
├── png_figures/                                # Static PNG visualizations for GitHub preview
│   ├── plot.png
├── iframe_figures/                             # Interactive HTML visualizations for Binder
│   ├── figure_20.html
│   ├── figure_21.html
├── requirements.txt                            # Python dependencies
└── README.md                                    # Project documentation (this file)
```
## Launch on Binder

This notebook includes interactive Plotly and Folium visualizations that may not render correctly on GitHub.  
To view the fully interactive version, launch it on Binder:

[![Launch Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/filipe-braiman/stock-data-extraction-visualization/HEAD)

## Methodology

### Data Extraction
- **API Integration**: Used `yfinance` library to extract historical stock data for Tesla and GameStop
- **Web Scraping**: Implemented web scraping with `BeautifulSoup` to extract revenue data from Macrotrends financial websites
- **Data Cleaning**: Processed and cleaned extracted data, handling currency formatting and missing values

### Visualization
- **Interactive Charts**: Created dual-panel interactive graphs using Plotly
- **Comparative Analysis**: Visualized both stock price movements and revenue trends simultaneously
- **Time Series Analysis**: Focused on data from 2011-2025 to capture significant market events

## Key Features

### Data Collection
- Real-time stock price data extraction via yfinance API
- Web scraping of financial revenue data from Macrotrends.net
- Automated data cleaning and preprocessing pipeline

### Visualization Capabilities
- Interactive stock price charts with range sliders
- Dual-panel displays showing both price and revenue trends
- Customizable time period analysis
- Professional financial chart styling

## Technologies and Libraries

* **Data Extraction**: yfinance, requests, BeautifulSoup
* **Data Manipulation**: pandas, numpy
* **Visualization**: plotly, plotly.graph_objects
* **Environment**: Jupyter Notebook

## Installation and Usage

### Prerequisites
- Python 3.7+
- Jupyter Notebook

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/stock-data-extraction-visualization.git
   cd stock-data-extraction-visualization
   ```

2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Open and run `Stock_Data_Extraction+Visualization.ipynb`

### Running the Analysis
Execute the notebook cells sequentially to:
- Extract Tesla stock data and revenue
- Extract GameStop stock data and revenue  
- Generate interactive visualizations
- View the exported HTML figures in the `iframe_figures` directory

## Code Overview

The project implements a reusable graphing function:

```python
def make_graph(stock_data, revenue_data, stock):
    # Creates dual-panel interactive visualization
    # showing historical share price and revenue trends
```

Key analysis steps include:
- Tesla stock data extraction using `yf.Ticker('TSLA')`
- Tesla revenue data scraping from Macrotrends
- GameStop stock data extraction using `yf.Ticker('GME')`
- GameStop revenue data scraping
- Interactive visualization generation for both companies

## Results

The project successfully:
- Extracted comprehensive historical data for both companies
- Created professional interactive visualizations
- Demonstrated the relationship between stock performance and revenue trends
- Provided insights into both companies' financial trajectories

## Author
**Filipe Braiman Carvalho**  
Applied AI & LLM Systems | Deep Learning · Transformers · RAG · Computer Vision | End-to-End ML Engineering

**Email:** [filipebraiman@gmail.com](mailto:filipebraiman@gmail.com)  
**LinkedIn:** [linkedin.com/in/filipe-b-carvalho](https://www.linkedin.com/in/filipe-b-carvalho)  
**GitHub:** [github.com/filipe-braiman](https://github.com/filipe-braiman)  

### About Me  
AI and data professional with experience in **LLM evaluation, retrieval-augmented generation (RAG), and AI model validation**. Currently working in **AI R&D at Huawei as an AI Evaluation Specialist**, contributing to the reliability and real-world performance of LLM and RAG systems. Strong background in **Python-based data and AI workflows**, including model assessment, dataset development, and analytical reporting for production-oriented AI solutions. Portfolio projects explore **deep learning architectures, computer vision, RAG systems, and applied machine learning experimentation**, emphasizing reproducible ML pipelines and practical AI engineering.

## Version History

| Version | Date       | Changes                 |
| :------ | :--------- | :---------------------- |
| 1.0     | 2025-10-29 | Initial Release.        |
| 1.1     | 2026-03-08 | Updated Author section. |
