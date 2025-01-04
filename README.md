
# Data Extraction and Text Analysis

This repository contains a project completed for Blackcoffer Consulting, aimed at extracting textual data from given URLs and performing text analysis. The project involves extracting article text, performing various analyses, and generating insights using Python.

## Table of Contents

- [Objective](#objective)
- [Technologies Used](#technologies-used)
- [Project Workflow](#project-workflow)
  - [Data Extraction](#data-extraction)
  - [Data Analysis](#data-analysis)
- [Output Variables](#output-variables)
- [Usage](#usage)
- [Folder Structure](#folder-structure)


---

## Objective

The primary goal of this project is to extract text articles from the provided URLs and compute analytical variables, including sentiment and readability metrics.

---

## Technologies Used

- Python
- Libraries: `BeautifulSoup`, `Selenium`, `Scrapy`, `pandas`, `numpy`, and others.

---

## Project Workflow

### Data Extraction

1. **Input**: The URLs are provided in `Input.xlsx`.
2. **Extraction**:
   - Articles are scraped using Python-based tools (`BeautifulSoup`, `Selenium`, or `Scrapy`).
   - Only the article title and text are extracted (excluding website headers, footers, and other non-content elements).
3. **Output**: The extracted content is saved in `.txt` files named using the `URL_ID`.

### Data Analysis

1. **Text Analysis**:
   - Compute variables such as sentiment scores, readability indices, and word statistics.
2. **Output Format**:
   - The results are saved in a structured format as defined in `Output Data Structure.xlsx`.

---

## Output Variables

The analysis produces the following variables:

- **POSITIVE SCORE**: Measure of positive sentiment.
- **NEGATIVE SCORE**: Measure of negative sentiment.
- **POLARITY SCORE**: Sentiment polarity.
- **SUBJECTIVITY SCORE**: Extent of subjectivity.
- **AVG SENTENCE LENGTH**
- **PERCENTAGE OF COMPLEX WORDS**
- **FOG INDEX**
- **AVG NUMBER OF WORDS PER SENTENCE**
- **COMPLEX WORD COUNT**
- **WORD COUNT**
- **SYLLABLE PER WORD**
- **PERSONAL PRONOUNS**
- **AVG WORD LENGTH**

Detailed definitions can be found in the `Text Analysis.docx` file.

---

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/varunsonawane/Data-Extraction-and-Text-Analysis.git
   cd Data-Extraction-and-Text-Analysis
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the scripts:
   - For data extraction:
     ```bash
     python extract_data.py
     ```
   - For data analysis:
     ```bash
     python analyze_data.py
     ```

4. Results are saved in a `.csv` or `.xlsx` format.

---

## Folder Structure

```
|-- BlackCoffer Internship Project/
    |-- Input.xlsx
    |-- Output Data Structure.xlsx
    |-- extract_data.py
    |-- analyze_data.py
    |-- README.md
    |-- outputs/
        |-- <Extracted Text Files>
        |-- analysis_results.csv
```






