# Raw Data

This directory contains information about the original source data used in this project.

The raw data originates from the PostgreSQL database **ads_analysis_goit_course** (schema `public`) and consists of four source tables representing daily advertising activity from Facebook Ads and Google Ads.

## Source Tables

### facebook_ads_basic_daily

Fact table containing daily Facebook Ads performance metrics, including:

* advertising date
* campaign ID
* ad set ID
* spend
* impressions
* reach
* clicks
* leads
* conversion value
* UTM URL

### facebook_campaign

Lookup table that maps Facebook campaign IDs to human-readable campaign names.

### facebook_adset

Lookup table that maps Facebook ad set IDs to audience segment names.

### google_ads_basic_daily

Fact table containing daily Google Ads performance metrics.

Unlike the Facebook dataset, campaign and ad set names are already stored as text values.

## Notes

The raw source tables are stored in the PostgreSQL database and are **not included** in this repository.

They were used as the input for the SQL data preparation process described in the `/sql` directory.

The processed analytical dataset generated from these source tables is available in the `/data/processed` directory.
