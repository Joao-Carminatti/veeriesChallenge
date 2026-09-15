# Veeries Challenge

> Technical challenge developed in Python involving the consumption of an external API and the processing of agricultural commodity data.

## 📋 About

This project was developed as part of a technical challenge for **Veeries**.

The application consumes data from the **USDA Foreign Agricultural Service Open Data API**, retrieves information about countries and commodities, identifies the required data, and exports the results to a CSV file.

The project was developed to demonstrate practical knowledge of:

* Python
* REST APIs
* HTTP requests
* JSON data
* Data processing
* Pandas
* CSV file generation
* Basic automation

## 🎯 Project Objective

The main objective of the challenge was to consume information from the USDA API and obtain export data for a specific agricultural commodity and selected countries.

The application:

1. Retrieves the available countries from the API.
2. Retrieves the available commodities.
3. Identifies **Soybean Oil**.
4. Identifies **China** and **Mexico**.
5. Requests the market year from the user.
6. Retrieves the export data for the selected market year.
7. Processes the returned information.
8. Exports the result to a CSV file.

## 🔄 Application Flow

```text
USDA Foreign Agricultural Service API
                  │
                  ▼
          Retrieve countries
                  │
                  ▼
         Retrieve commodities
                  │
                  ▼
        Identify Soybean Oil
                  │
                  ▼
       Identify China and Mexico
                  │
                  ▼
        Select Market Year
                  │
                  ▼
       Retrieve export data
                  │
                  ▼
         Process the results
                  │
                  ▼
            Generate CSV
```

## 🛠️ Technologies

* **Python**
* **Requests** — HTTP requests and API communication
* **Pandas** — data processing and CSV generation
* **Schedule** — execution scheduling
* **USDA Foreign Agricultural Service Open Data API**

## 📁 Project Structure

```text
veeriesChallenge/
│
├── README.md
├── outputfile.csv
├── requirements.txt
└── routine.py
```

### `routine.py`

Main Python script responsible for:

* Connecting to the USDA API
* Retrieving countries
* Retrieving commodities
* Finding the codes for the required countries and commodity
* Requesting export data
* Processing the API responses
* Generating the CSV output
* Scheduling the routine execution

### `outputfile.csv`

CSV file containing the data obtained from the API and exported by the application.

### `requirements.txt`

Contains the Python dependencies used by the project.

## 🚀 Getting Started

### Prerequisites

Make sure you have Python installed on your machine.

### 1. Clone the repository

```bash
git clone https://github.com/Joao-Carminatti/veeriesChallenge.git
```

Enter the project directory:

```bash
cd veeriesChallenge
```

### 2. Install the dependencies

Install the packages listed in `requirements.txt`:

```bash
pip install -r requirements.txt
```

### 3. Run the application

Execute the Python script:

```bash
python routine.py
```

The application will request the **Market Year** through the terminal and then communicate with the USDA API to retrieve the corresponding information.

## 📊 Output

The application generates a CSV file named:

```text
outputfile.csv
```

The file contains information returned by the USDA API, including data related to:

* Commodity
* Country
* Weekly exports
* Accumulated exports
* Outstanding sales
* Gross new sales
* Current market year net sales
* Current market year total commitment
* Next market year outstanding sales
* Next market year net sales
* Unit
* Week ending date

## 🌎 Data Source

The project uses the **USDA Foreign Agricultural Service Open Data API** to retrieve agricultural trade information.

The API provides data related to commodities, countries and export activity.

## 🧠 What I Learned

Through this challenge, I gained practical experience with:

* Consuming external REST APIs
* Making HTTP requests with Python
* Working with JSON responses
* Searching and filtering API data
* Extracting specific information from structured responses
* Processing data using Pandas
* Generating CSV files
* Working with API-based data pipelines
* Automating the execution of Python routines

## 📌 Project Context

This repository was originally developed as a **technical challenge for a position at Veeries**.

It is maintained as part of my development portfolio to demonstrate practical experience with **Python, APIs, data processing and system integration**.

## 👨‍💻 Author

**João Gabriel Braz Carminatti**

Developer focused on **Back-End Development, APIs, System Integration and Automation**.

* GitHub: https://github.com/Joao-Carminatti
* LinkedIn: https://www.linkedin.com/in/joaocarminatti/
