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

## Correlation

CORR([monthly_spend],
[monthly_leads])
