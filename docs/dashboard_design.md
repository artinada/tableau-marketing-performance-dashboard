# Dashboard Design

## Design Goals

The dashboard was designed to provide executives with a single-page overview of marketing performance.

The layout follows a top-down analytical flow.


## KPI Section

Top row contains high-level KPIs:

- Spend
- Impressions
- Clicks
- Leads
- CTR
- CPC
- CPL
- CPM
- ROMI

---

### Main Analytical Section

The central part of the dashboard includes four main visualizations.

#### 1. Spend vs Leads Analysis

A dual-axis chart showing:

* monthly advertising spend;
* monthly number of leads;
* correlation between monthly spend and leads.

This chart helps evaluate whether increased advertising budget is associated with increased lead generation.

#### 2. Metric Trend

A line chart showing how the selected marketing metric changes over time for Facebook and Google.

This allows direct comparison of advertising platforms.

#### 3. Campaign Ranking

A horizontal bar chart ranking campaigns by the selected metric.

Campaigns are sorted in descending order to quickly identify top-performing campaigns.

#### 4. Campaign Efficiency Analysis

A scatter plot showing the relationship between advertising spend and campaign efficiency.

Chart logic:

* each point represents one campaign;
* X-axis: advertising spend;
* Y-axis: selected metric;
* color: advertising source;
* size: number of leads.

---

## Dashboard Interactivity

The dashboard includes:

- parameter switching
- dashboard filter actions
- campaign drill analysis
- cross-filtering

When a user clicks a campaign in the `Campaign Efficiency Analysis` scatter plot, the following charts are filtered by the selected campaign:

* `Metric Trend`
* `Spend vs Leads Analysis`

The action uses `campaign_name` as the selected field for filtering.

---

## Dashboard Filters

The dashboard includes the following filters:

* date period;
* source;
* campaign name;
* adset name / audience segment;
* UTM campaign.

The date filter is displayed by month.
