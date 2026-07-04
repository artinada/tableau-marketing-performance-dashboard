# Processed Data

This directory contains the final analytical dataset used for building the Tableau Public dashboard.

The dataset was created by transforming and combining multiple advertising data sources using SQL in PostgreSQL.

## Dataset

### `marketing_ads_dataset.csv`

This file contains the consolidated marketing dataset prepared for business intelligence and visualization.

The data preparation process description: /docs/data_preparation.md

## Included Fields

The processed dataset includes the following fields:

| Field               | Description                               |
| ------------------- | ----------------------------------------- |
| `ad_date`           | Advertising activity date                 |
| `source`            | Advertising platform (Facebook or Google) |
| `campaign_name`     | Campaign name                             |
| `adset_name`        | Ad set / audience segment                 |
| `utm_campaign`      | Decoded UTM campaign parameter            |
| `total_spend`       | Total advertising spend                   |
| `total_impressions` | Number of ad impressions                  |
| `total_reach`       | Number of users reached                   |
| `total_clicks`      | Number of ad clicks                       |
| `total_leads`       | Number of generated leads                 |
| `total_value`       | Marketing value (profit)                  |

## Purpose

The processed dataset serves as the single source of truth for all visualizations, calculated fields, parameters, and dashboard interactions implemented in Tableau Public.

## Related Files

* SQL queries used to generate the dataset are available in the `/sql` directory.
* Dashboard visualizations are available in the `/tableau` directory.
* Project documentation can be found in the `/docs` directory.
