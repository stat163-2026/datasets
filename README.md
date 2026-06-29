# STAT163 datasets

Public datasets used by STAT163 practice notebooks (loaded directly by URL via raw.githubusercontent).

## online_retail/

UCI **Online Retail II** — UK online-retail transactions, split by year and gzipped.
Source: https://archive.ics.uci.edu/dataset/502/online+retail+ii

- `online_retail_2009.csv.gz` — 525,461 rows (sheet "Year 2009-2010")
- `online_retail_2010.csv.gz` — 541,910 rows (sheet "Year 2010-2011"); December 2010 overlaps the 2009 file by design.

Columns: `Invoice, StockCode, Description, Quantity, InvoiceDate, Price, Customer ID, Country`.

## moma/

**MoMA collection** — Museum of Modern Art artworks; human-entered fields with messy text, heterogeneous dates, and missing values.
Source: https://github.com/MuseumofModernArt/collection

- `artworks.csv.gz` — 160,597 rows (full export, 15 columns kept).

Columns: `Title, Artist, Nationality, Date, Medium, Dimensions, AccessionNumber, Classification, Department, DateAcquired, Height (cm), Width (cm), Depth (cm), Diameter (cm), Duration (sec.)`.

## arxiv/

**arXiv metadata** — preprints split by submission year and gzipped, in two clusters by primary (first) category. Packed multi-value categories, free-text abstracts, raw `authors` (`"A, B and C"`, affiliations in parens), messy `comments`.
Source: https://www.kaggle.com/datasets/Cornell-University/arxiv

- `arxiv_aiml_2018.csv.gz` … `arxiv_aiml_2024.csv.gz` — **AI/ML** cluster (`cs.LG`, `cs.CV`, `cs.CL`, `cs.AI`, `cs.NE`, `stat.ML`): 18,910 / 25,009 / 32,154 / 36,640 / 39,918 / 51,502 / 66,501 rows (270,634 total).
- `arxiv_econ_2018.csv.gz` … `arxiv_econ_2024.csv.gz` — **economics** cluster (`econ.*`): 458 / 670 / 1,069 / 1,371 / 1,321 / 1,468 / 1,740 rows (8,097 total).

Columns: `id, submitted_date, categories, title, abstract, authors, num_authors, comments, journal_ref`. Only whitespace is collapsed in text fields; categories stay packed and `comments`/`journal_ref` stay as-is (missingness preserved).
