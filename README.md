# Trendsetter Detection in the Iowa Liquor Market
The Data Incubator  
2020 Fall  
Capstone Project

# 1 Business Objective

# 2 Data Ingestion

|      | dtype          |    count |   null count |   unique | top                 |   freq | first               | last                |
|:-----|:---------------|---------:|-------------:|---------:|:--------------------|-------:|:--------------------|:--------------------|
| Date | datetime64[ns] | 19883991 |            0 |     2157 | 2017-12-22 |  16674 | 2012-01-03 | 2020-10-30 |

|                 | dtype   |    count |   null count |   unique | top                          |     freq |
|:----------------|:--------|---------:|-------------:|---------:|:-----------------------------|---------:|
| Invoice         | object  | 19883991 |            0 | 19883991 | 128404200011                 |        1 |
| Store_num       | object  | 19883991 |            0 |     2495 | 2633                         |   169816 |
| Store           | object  | 19883991 |            0 |     2613 | Hy-Vee #3 / Bdi / Des Moines |   169816 |
| Address         | object  | 19804064 |        79927 |     2415 | 3221 Se 14Th St              |   231054 |
| City            | object  | 19804065 |        79926 |      456 | Des Moines                   |  1730907 |
| Zip             | object  | 19804020 |        79971 |      489 | 50010                        |   491093 |
| County_num      | object  | 19727260 |       156731 |      108 | 77                           |  3622703 |
| County          | object  | 19727262 |       156729 |      104 | Polk                         |  3622703 |
| Subcategory_num | object  | 19867017 |        16974 |      110 | 1012100                      |  1916720 |
| Subcategory     | object  | 19858951 |        25040 |      110 | Canadian Whiskies            |  1916720 |
| Vendor_num      | object  | 19883991 |            0 |      362 | 260                          |  3356016 |
| Vendor          | object  | 19883991 |            0 |      452 | Diageo Americas              |  3356016 |
| Item_num        | object  | 19883991 |            0 |     9774 | 11788                        |   200245 |
| Item            | object  | 19883991 |            0 |     8666 | Black Velvet                 |   515736 |
| Category        | object  | 19597340 |       286651 |        9 | Whiskey                      |  5394096 |
| Anomalous       | bool    | 19883991 |            0 |        2 | False                        | 18409105 |

|               | dtype   |    count |   null count |   mean |   std |   min |   0.01% |   99.99% |      max |
|:--------------|:--------|---------:|-------------:|-------:|------:|------:|--------:|---------:|---------:|
| Bottle_pack   | int16   | 19883991 |            0 |     12 |     8 |     1 |       1 |       48 |      336 |
| Bottle_mL     | int32   | 19883991 |            0 |    911 |   663 |     0 |      50 |     3600 |   378000 |
| Bottle_cost   | int32   | 19883991 |            0 |    995 |  1074 |     0 |       0 |    14525 |   768000 |
| Bottle_retail | int32   | 19883991 |            0 |   1494 |  1610 |     0 |       0 |    21788 |  1152000 |
| Bottle_count  | int16   | 19883991 |            0 |     10 |    28 |     0 |       1 |      804 |    15000 |
| Cents         | int32   | 19883991 |            0 |  13527 | 47022 |     0 |       0 |  1620000 | 27955728 |
| mL            | int32   | 19883991 |            0 |   9137 | 33778 |     0 |      50 |  1050000 | 15000000 |
| Gallons       | float32 | 19883991 |            0 |      2 |     9 |     0 |       0 |      277 |     3963 |
| Longitude     | float32 | 17976922 |      1907069 |    -91 |     3 |  -105 |     -97 |      -90 |      -74 |
| Latitude      | float32 | 17976922 |      1907069 |     42 |     1 |    39 |      40 |       43 |       45 |
| Random | float64 | 19883991 |            0 |    0.5 |   0.3 |   0 |     0 |      1 |   1 |







# 3 Visualization

# 4a Machine Learning

# 4b Distributed Computing

# 4c Interactive Website

# 5 Deliverable
This current [README](README.md)
