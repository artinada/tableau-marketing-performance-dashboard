# Calculated Fields

## CTR

Measures the percentage of users who clicked an advertisement.

CTR =
Clicks / Impressions

---

## CPC

Average advertising cost per click.

CPC =
Spend / Clicks

---

## CPM

Advertising cost per 1000 impressions.

CPM =
Spend / Impressions × 1000

---

## CPL

Average cost per generated lead.

CPL =
Spend / Leads

---

## ROMI

Return on marketing investment.

ROMI =
Value / Spend

---

## Clicks to Leads Conversion

Leads / Clicks

---

## Reach to Leads Conversion

Leads / Reach

---

## Monthly Spend (LOD)

{ FIXED DATETRUNC('month',[ad_date]) :
SUM([Spend])
}

---

## Monthly Leads (LOD)

{ FIXED DATETRUNC('month',[ad_date]) :
SUM([Leads])
}

---

## Parameter: Select Metric

The dashboard includes a parameter called `Select Metric`, which allows users to switch dynamically between marketing metrics.

Available metric options:

* CTR
* CPC
* CPL
* ROMI
* Clicks to Leads Conversion
* Reach to Leads Conversion

The parameter is connected to the calculated field `Selected Metric`.

```tableau
CASE [Select Metric]
WHEN "CTR" THEN [CTR]
WHEN "CPC" THEN [CPC]
WHEN "CPL" THEN [CPL]
WHEN "ROMI" THEN [ROMI]
WHEN "Clicks to Leads Conversion" THEN [Clicks to Leads Conversion]
WHEN "Reach to Leads Conversion" THEN [Reach to Leads Conversion]
END
```


## Correlation

CORR([monthly_spend],
[monthly_leads])
