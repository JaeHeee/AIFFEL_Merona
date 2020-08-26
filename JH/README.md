# AIFFEL_Merona

<br>


## EDA

- 연말에 가격 판매량 증가
- 특정 카테고리가 많이 팔린다.
- 3개정도의 가게가 판매량이 높고, 나머지는 비슷
- item_price, item_cnt에 outlier 있다.  

#### Possible item_id features:
1. Lags
2. Release date
3. Last month sale
4. Days on sale
5. Neighbors (items with id 1000 and 1001 could be somehow similar - genre, type, release date)  

- 새로 연 가게나 6개월 동안 판매량 없는 가게들 있다.

#### Possible shop_id features
1. Lags (shop_id/shp_cnt_mth)
2. Opening month (possible opening sales)
3. Closed Month (possible stock elimination)  

#### Possible Price features
1. Price category (1 /10 /20$/ etc.) - obviously (or not obviously), items with smaller price have greater volumes
2. Discount and Discount duration
3. Price lag (shows discount)
4. Price correction (rubl/usd pair)
5. Shop Revenue  

#### Possible Date features:
1. Weekends and holidays sales (to correct monthly sales)
2. Number of days in the month (to correct monthly sales)
3. Month number (for seasonal items)  

#### Possible Shop features
1. Shop City
2. Shop Type  

#### Possible Item features
1. Item name
2. Encoded aditional feature  

#### Possible Category features
1. Section
2. Main Category name
3. Main SubCategory name
4. Secondary SubCategory name  

The key of success is the analysis of Test test data.  

We have three groups of items  
  
- Item/shop pairs that are in train
- Items without any data
- Items that are in train
