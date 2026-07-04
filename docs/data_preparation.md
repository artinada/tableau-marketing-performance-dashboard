# Data Preparation

## Source Data

The project uses four PostgreSQL tables:

- facebook_ads_basic_daily
- facebook_campaign
- facebook_adset
- google_ads_basic_daily

## Preparation Workflow

1. explore source tables and column types;
2. identify fact tables and lookup tables;
3. join Facebook Ads data with campaign and adset dictionaries;
4. standardize field names;
5. unify Facebook and Google Ads data using `UNION ALL`;
7. added the `source` field to distinguish advertising platforms;
8. decoded UTM campaign parameters;
9. handle null values using `COALESCE`;
10. calculate core aggregated metrics;
11. exported the final dataset to CSV;
12. import the CSV file into Tableau Public.

## Technologies

- PostgreSQL
- SQL
- DBeaver
