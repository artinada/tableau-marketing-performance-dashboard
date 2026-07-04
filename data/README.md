# Data Folder

This directory contains the analytical dataset used to build the Tableau dashboard.

## Dataset

**marketing_ads_dataset.csv**

The dataset was generated from the PostgreSQL database `ads_analysis_goit_course` after preparing and combining advertising data from multiple source tables.

The data preparation process included:

* joining Facebook Ads data with campaign and ad set lookup tables;
* combining Facebook Ads and Google Ads into a single dataset;
* replacing missing values using `COALESCE`;
* decoding UTM campaign parameters;
* calculating aggregated marketing metrics;
* exporting the final result to CSV for Tableau Public.

## Data Sources

The original dataset was created from the following database tables:

* `facebook_ads_basic_daily`
* `facebook_campaign`
* `facebook_adset`
* `google_ads_basic_daily`

## Main Fields

The exported dataset contains:

* `ad_date`
* `source`
* `campaign_name`
* `adset_name`
* `utm_campaign`
* `total_spend`
* `total_impressions`
* `total_reach`
* `total_clicks`
* `total_leads`
* `total_value`

## Notes

The original database is part of the educational dataset provided for the GoIT Data Analytics course.

Only the processed analytical dataset is included in this repository. The SQL queries used to generate the dataset are available in the `/sql` directory.
