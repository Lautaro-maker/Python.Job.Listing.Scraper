# Python.Job.Listing.Scraper
Python web scraper that collects job listings from the Fake Python Jobs website. This scraper extract information such as the job title, company name, location, and a link to the full job description. The project page where the task is located :https://roadmap.sh/projects/job-listings-scraper

# 🕷️ Job Listings Web Scraping
**User Guide and Project Documentation**

## 📖 Project Description
This project consists of a Python script developed using the **Jupyter Notebook** interactive environment. Its main objective is to automatically extract detailed information about job postings from a specific website and structure it into a clean tabular format.

The extracted data is processed, cleaned of unnecessary spaces and line breaks (messy code), and exported directly to a `.csv` file, making it ready for analysis in tools like Excel, Google Sheets, Pandas, or PowerBI.

## 🛠️ Technologies and Libraries Used
* **Python 3**: Main programming language.
* **Jupyter Notebook**: Interactive development environment.
* **BeautifulSoup (bs4)**: Library used to parse, navigate, and extract specific data from the website's HTML structure.
* **Requests**: Library in charge of making HTTP requests and downloading the source code.
* **CSV (Python Standard Library)**: For iterating, generating, and writing the final output file.

## ⚙️ Requirements and Installation
To run this project in your local environment, make sure you have Python installed. Then, follow these steps:

1. **Clone the repository:** Download the code from GitHub to your computer using the terminal:
   ```bash
   git clone [YOUR_REPOSITORY_URL]
   cd [PROJECT_FOLDER_NAME]
   ```
2. **Install necessary dependencies:** Make sure to install the required libraries by running the following command:
   ```bash
   pip install beautifulsoup4 requests jupyter
   ```

## 🚀 How to Run the Project
Since the source code is in an interactive file, you must start it via the Jupyter server:

1. Open your terminal in the root folder where the project is located.
2. Start the local Jupyter Notebook server:
   ```bash
   jupyter notebook
   ```
3. A tab will open in your web browser. Click on the main file (the one with the `.ipynb` extension).
4. Run the code cells in sequential order (you can use `Shift + Enter` cell by cell or run all from the menu).

## 📊 Output Data Structure
Upon completing the execution of the last code block, a file named `Job.Listing.Scrap.csv` will be automatically generated in the same project folder. This file contains the information organized in the following columns:

| Column | Description |
| :--- | :--- |
| **Job Title** | The official title or position of the job offer. |
| **Company Name** | The name of the company posting the vacancy. |
| **Location** | The location (city, state, country) where the position is offered. |
| **Link** | Direct URL to access the full description and apply for the offer. |

> **Technical Note:** The script incorporates cleaning and specific selection routines. The `.strip()` method is used to ensure that the extracted texts do not contain indentations or residual whitespace from the original HTML. Additionally, specific text filters (`string='Apply'`) are applied to guarantee that the collected links are the correct ones and not secondary buttons.
