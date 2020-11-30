# Segmenting the Iowa Wholesale Liquor Market

The Data Incubator  
2020 Fall  
Capstone Project

# 1 Business Objective

Wholesale liquor is a 300 million dollar a year market [See Table 1]
with 452 sellers (brands/manufacturers)
and 2415 buyers (liquor stores) [See Note 1].
Wholesale transactions 
are reported to the Iowa Alcoholic Beverages Division,
who make the data (from 2012 to present) available at:
https://data.iowa.gov/Sales-Distribution/Iowa-Liquor-Sales/m3tr-qhgy  
https://data.iowa.gov/api/views/m3tr-qhgy/rows.csv?accessType=DOWNLOAD

The dataset consists of about 19 million transactions
from 2012 through the present, and is about 4.5 GB [See Table 2 below].

Each liquor store typically carries around 35 brands (see table below),
and each brand employs salespersons that work the a number of liquor stores.
For context, in the Manhattan liquor market, a salesperson
might have a territory of 50 liquor stores.

This product uses machine learning
(feature engineering and density-based clustering)
to partition the iowa liquor market into discrete components.
Market segmentation will benefit wholesalers (the intended user) by allowing them to:
- target advertising by region
- identify potential buyers (liquor stores)
- more effectively partition sales regions for salespersons

#### Note 1
Note that the Iowa wholesale market excludes
on-premise retailers (ie, restaurants and bars),
who must buy through an off-premise retailer (ie, a liquor store).

#### Table 1

|                    |   Brandy |   Cocktail |   Gin |   Liqueur |   Neutral |   Rum |   Tequila |   Vodka |   Whiskey |    All |
|:-------------------|---------:|-----------:|------:|----------:|----------:|------:|----------:|--------:|----------:|-------:|
| USD (Millions)     |    14.58 |       4.37 |  7.27 |     44.82 |      0.85 | 32.95 |     19.77 |   73.73 |     99.17 | 297.50 |
| Liters (Millions)  |     0.60 |       0.60 |  0.49 |      2.65 |      0.04 |  2.34 |      0.85 |    6.28 |      5.19 |  19.05 |
| Gallons (Millions) |     0.16 |       0.16 |  0.13 |      0.70 |      0.01 |  0.62 |      0.22 |    1.66 |      1.37 |   5.02 |

#### Table 2

|                       | filename           | filesize | number of rows |
|:----------------------|-------------------:|---------:|---------------:|
| Raw data              |            raw.csv |     4.5G |       19 884 006 |
| Cleaned data          |       data.parquet |     848M |       19 883 991 |
| _nonanomalous rows only_|                  |          |     _18 409 105_ |
| Downsampled data (5%) | downsample.parquet |      47M |         993 222 |



# 2 Data Ingestion

The dataset after cleaning and formatting (but before feature engineering)
has 25 columns, including the following.

|      | dtype          |    count |   null count |   unique | top                 |   freq | first               | last                |
|:-----|:---------------|---------:|-------------:|---------:|:--------------------|-------:|:--------------------|:--------------------|
| Date | datetime64[ns] | 19883991 |            0 |     2157 | 2017-12-22 |  16674 | 2012-01-03 | 2020-10-30 |
| Invoice         | object  | 19883991 |            0 | 19883991 | 128404200011                 |        1 |
| Store           | object  | 19883991 |            0 |     2613 | Hy-Vee #3 / Bdi / Des Moines |   169816 |
| Address         | object  | 19804064 |        79927 |     2415 | 3221 Se 14Th St              |   231054 |
| City            | object  | 19804065 |        79926 |      456 | Des Moines                   |  1730907 |
| Subcategory     | object  | 19858951 |        25040 |      110 | Canadian Whiskies            |  1916720 |
| Vendor          | object  | 19883991 |            0 |      452 | Diageo Americas              |  3356016 |
| Item            | object  | 19883991 |            0 |     8666 | Black Velvet                 |   515736 |

|               | dtype   |    count |   null count |   mean |   std |   min |   0.01% |   99.99% |      max |
|:--------------|:--------|---------:|-------------:|-------:|------:|------:|--------:|---------:|---------:|
| Cents         | int32   | 19883991 |            0 |  13527 | 47022 |     0 |       0 |  1620000 | 27955728 |
| Gallons       | float32 | 19883991 |            0 |      2 |     9 |     0 |       0 |      277 |     3963 |
| Longitude     | float32 | 17976922 |      1907069 |    -91 |     3 |  -105 |     -97 |      -90 |      -74 |
| Latitude      | float32 | 17976922 |      1907069 |     42 |     1 |    39 |      40 |       43 |       45 |

# 3 Visualization

# 4 Machine Learning

## Feature Engineering

## Clustering

# 5 Deliverable
The current [README](README.md)
