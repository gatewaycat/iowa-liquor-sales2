# Trendsetter Detection in the Iowa Liquor Market

The Data Incubator  
2020 Fall  
Capstone Project

# 1 Business Objective

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
