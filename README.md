# InvestLens | Real Estate Investment Analytics

InvestLens is a decision-support project for evaluating real estate investments in Egypt’s New Administrative Capital. It compares projects using a 100-point score, estimated fair values, and market scenarios.

[Download the project presentation](./InvestLens-Presentation.pptx)

## Business Problem

Investors need to compare property prices alongside location, developer track record, infrastructure, services, and payment terms. InvestLens brings these factors together to explain why a deal may be worth buying, negotiating, or avoiding.

## Data and Preparation

The project covers property characteristics, developer profiles, asking and comparable prices, payment plans, and local services. The SQL Server design organizes the data for analysis and reporting. Data preparation includes handling missing values, removing duplicates, standardizing area names, and checking relationships between tables.

## Decision Framework

| Component | Purpose |
|---|---|
| Capital Score | Rates projects out of 100 based on location, developer strength, infrastructure, services, liquidity, and payment terms. |
| Fair Value | Uses a machine learning approach to estimate fair value per square meter and compare it with the asking price. |
| Market Outlook | Explores alternative market scenarios through 2030. |
| Pricing Confidence | Accounts for the reliability of available pricing data. |
| Investor Preferences | Considers the investor’s budget, objective, preferred location, and payment preferences. |

## Example Recommendation

In an illustrative case, the asking price is EGP 42,000 per square meter and the estimated fair value is EGP 37,500. The asking price is 12% above the estimate. If the project has a strong developer and a good location, the framework recommends **Negotiate** and explains why.

## Reporting and Architecture

The presentation outlines Power BI dashboards for market trends, pricing opportunities, valuation, and developer comparisons. It also describes an application design in which a backend API connects SQL Server data to the scoring and recommendation engines, with results shown in a React interface.

## Next Steps

Expand the historical transaction dataset, validate fair-value estimates against actual sales, and add more frequent market updates.
