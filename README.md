
## 📘 CodeAlpha Internship — Task 1: Web Scraping

### 🧠 Project Title: **Books Data Scraper from BooksToScrape.com**

---

### 📝 **Project Description**

This project is part of the **CodeAlpha Data Analytics Internship**.
The goal of this task is to collect and analyze book data from the website [Books to Scrape](http://books.toscrape.com/).
Using Python and libraries like **BeautifulSoup**, **Requests**, and **Pandas**, we scrape multiple pages to extract book details such as:

* 📚 **Title**
* 💰 **Price**
* ⭐ **Rating**

After collecting the data, it’s cleaned, saved into a CSV file, and visualized to gain insights about book prices and ratings.

---

### ⚙️ **Technologies Used**

* Python 🐍
* BeautifulSoup (for parsing HTML)
* Requests (for HTTP requests)
* Pandas (for data manipulation)
* Matplotlib (for visualization)

---

### 🚀 **Steps Performed**

1. Sent HTTP requests to multiple pages of the website.
2. Extracted book titles, prices, and ratings using BeautifulSoup.
3. Stored the data in a Pandas DataFrame.
4. Cleaned and formatted the price column.
5. Saved the dataset as `books_dataset.csv`.
6. Created a bar chart showing **average price per rating**.

---

### 📊 **Key Insights**

* The website contains multiple books across different categories.
* Average book prices vary by rating.
* This dataset can be expanded for advanced analysis or sentiment detection using reviews.

---

### 📈 **Visualization Example**

```python
avg_prices = df.groupby('Rating')['Price'].mean()
avg_prices.plot(kind='bar', title='Average Book Price by Rating')
plt.xlabel('Rating')
plt.ylabel('Average Price (£)')
plt.show()
```

---

### 💾 **Dataset**

The dataset generated from this project is saved as:

```
books_dataset.csv
```

Columns include:

| Title | Price | Rating |
| ----- | ----- | ------ |

---

### 🧩 **How to Run**

1. Clone this repository
2. Install the dependencies:

   ```bash
   pip install requests beautifulsoup4 pandas matplotlib
   ```
3. Run the notebook or script:

   ```bash
   python books_scraper.py
   ```
4. The final dataset (`books_dataset.csv`) will be generated in the working directory.

---

### 🏁 **Output Example**

* ✅ `books_dataset.csv` file with scraped data
* 📈 A visualization showing average prices by rating
* 💬 A list of the cheapest 10 books

---

### 👩‍💻 **Intern Details**

**Name:** [mennatallah taha tawfiq]
**Program:** CodeAlpha Data Analytics Internship
**Duration:** October 20 – November 20, 2025

---

