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
