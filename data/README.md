# Data Folder

This directory contains the analytical dataset used to build the Tableau dashboard.

## Final Dataset

**marketing_ads_dataset.csv**

This dataset was generated from the PostgreSQL database `ads_analysis_goit_course` after preparing and combining advertising data from multiple source tables.

The data preparation process description: `/docs/data_preparation.md`

## Data Sources

The original dataset was created from the following database tables:

* `facebook_ads_basic_daily`
* `facebook_campaign`
* `facebook_adset`
* `google_ads_basic_daily`

Facebook campaign and adset names were joined from lookup tables using `campaign_id` and `adset_id`. Google Ads data already contained campaign and audience segment names.

## Notes

The original database is part of the educational dataset provided for the GoIT Data Analytics course.

Only the processed analytical dataset is included in this repository. The SQL queries used to generate the dataset are available in the `/sql` directory.
