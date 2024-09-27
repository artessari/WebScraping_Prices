<h1>Monthly Surveys - Widely Consumed Goods and Services</h1>
<h2>Data Collection Through Web Scraping</h2>

This repository contains a Jupyter notebook that extracts and analyzes the prices of widely consumed goods and services across all Italian provinces from the year 2021. The data is collected through automated web scraping from the [Osservaprezzi](https://osservaprezzi.mise.gov.it/prezzi/livelli/beni-e-servizi-di-largo-consumo/archivio-rilevazioni-beni-e-servizi-di-largo-consumo) website, which provides comprehensive information on pricing trends. Users can easily customize their data extraction by selecting specific months and provinces, simply by adjusting highlighted parameters within the code. The collected data is subsequently organized into a structured tabular format suitable for further analysis.

This code is designed for web scraping data on prices for widely consumed goods and services in Italy from the **Price and Tariffs Observatory** maintained by the Ministry of Enterprises and Made in Italy. It retrieves monthly price data for different types of products across various provinces, specifically focusing on the province of Bolzano. The scraped data is then organized and stored in structured formats, such as CSV and Excel files, making it easy to analyze and visualize trends in consumer pricing over time.

The code functions by making HTTP requests to the specified URL with user-defined parameters such as year, month, product type, and province. It employs the `requests` library to handle the requests and the `BeautifulSoup` library to parse the HTML response. The relevant data is extracted from HTML tables and stored in lists, which are then converted into a pandas DataFrame for further manipulation and analysis. This process allows for efficient and automated data collection over a specified time range.

This code was developed during an internship at [**ASTAT**](https://astat.provincia.bz.it/it/default.asp) (Provincial Institute of Statistics of Bolzano). The extracted data serves as the foundation for a publication on the prices of high-consumption goods and services in South Tyrol and Italy.

## Repository Structure

```
├── dati_prezzi.ipynb                           # Main Jupyter notebook containing the data extraction and analysis code
├── results/                                    # Directory for example output files
│   ├── prezzi_BZ_2021-01_2024-07.xlsx          # Sample prices for Bolzano from January 2021 to July 2024
│   ├── prezzi_province_2022-01_2022-12.xlsx    # Sample prices for all provinces from January to December 2022
│   ├── prezzi_province_2023-01_2023-12.xlsx    # Sample prices for all provinces from January to December 2023
│   └── prezzi_province_2024-01_2024-07.xlsx    # Sample prices for all provinces from January to July 2024
├── requirements.txt                            # Dependencies for the project (used to recreate the environment)
└── README.md                                   # Project README file providing an overview and instructions

```

## Key Files

- MLProject_TessariArianna_19322.ipynb: The main notebook that contains data preprocessing, exploratory data analysis (EDA), model training, and evaluation.
- in-vehicle-coupon-recommendation.csv: The dataset used for training and testing the models.
- MLReport_TessariArianna_19322.pdf: A detailed report that discusses the objectives, methodology, and conclusions.
- requisites.txt: The list of Python dependencies required to run the project.

## How to Run

**1. Clone the repository**
```
git clone https://github.com/artessari/WebScraping_Prices
cd WebScraping_Prices
```

**2. Install Dependencies**

To install the required Python libraries, run:
```
pip install -r requisites.txt
```

**3. Run Jupyter Notebook**

To explore the project interactively, launch the notebook.

### References
**ISTAT** - Italian National Institute of Statistics  
**Ministry of Enterprises and Made in Italy**  
**Price and Tariffs Observatory**  
Source for Web Scraping: https://osservaprezzi.mise.gov.it/prezzi/livelli/beni-e-servizi-di-largo-consumo/archivio-rilevazioni-beni-e-servizi-di-largo-consumo
