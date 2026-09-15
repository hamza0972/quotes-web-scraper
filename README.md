# Quotes Web Scraper

A Python web scraper that extracts quotes, authors, and tags from [Quotes to Scrape](https://quotes.toscrape.com/).

This project demonstrates practical web scraping using Python, Requests, and BeautifulSoup, including pagination, HTML parsing, data extraction, and CSV file handling.

---

## 📌 Project Overview

The scraper automatically collects quote data from multiple pages of the website.

For each quote, it extracts:

- Quote text
- Author name
- Associated tags

The scraper continues navigating through the available pages until there are no more pages to scrape, then saves the collected data into a CSV file.

---

## 🚀 Features

- Scrapes data from multiple web pages
- Extracts quote text
- Extracts author names
- Extracts quote tags
- Handles website pagination automatically
- Parses HTML using BeautifulSoup
- Sends HTTP requests using Requests
- Stores structured data in CSV format
- Handles multiple tags for each quote
- Can be run using Jupyter Notebook or Google Colab

---

## 🛠️ Technologies Used

- **Python**
- **Requests**
- **BeautifulSoup**
- **CSV**
- **Jupyter Notebook**
- **Google Colab**

---

## 📊 Data Extracted

The scraper collects the following information:

| Field | Description |
|---|---|
| Quote | Text of the quote |
| Author | Author of the quote |
| Tags | Tags associated with the quote |

### Example

| Quote | Author | Tags |
|---|---|---|
| “The world as we have created it is a process of our thinking...” | Albert Einstein | change, deep-thoughts, thinking, world |

---

## 🔄 How It Works

The scraping workflow is:

```text
Website
   ↓
Send HTTP Request using Requests
   ↓
Receive HTML Response
   ↓
Parse HTML using BeautifulSoup
   ↓
Find Quote Elements
   ↓
Extract Quote, Author and Tags
   ↓
Check for Next Page
   ↓
Follow Next Page
   ↓
Repeat Until No More Pages
   ↓
Store Data in CSV
