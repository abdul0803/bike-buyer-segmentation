# Bike Sales Analysis — Case Study
Live workbook: https://docs.google.com/spreadsheets/d/1T4JwgoOAV5ApoU7WsM6qygHvV8hnIGtn9uBhGnCmhG4/edit?usp=sharing

## Business Question
Which customer segment is most likely to purchase a bike, and what factors — age, income, or family size — actually drive that likelihood?

## Data
Bike buyers dataset (~1,026 customers). Key fields used: Gender, Income, Age (bucketed into Adolescent / Middle age / Old), Number of Children, Education, Commute Distance, and Purchased Bike (Yes/No).

## Approach
Built pivot tables and charts in Google Sheets to compare purchase behavior across gender, age bracket, income, education, commute distance, and number of children. Rather than relying on raw purchase counts — which are skewed by how many customers fall into each group — purchase **rate** (% who bought, within each group) was calculated to isolate real behavioral differences from simple group-size effects.

## Findings

**Age bracket is the strongest driver.** Middle-age customers convert at 54.7%, compared to 36.6% for Adolescent and 31.3% for Old — nearly double the next-closest group. This holds even after controlling for the fact that middle-age is also the largest customer segment overall.

**Income matters, but only within the middle-age segment.** Overall average income looked similar between buyers and non-buyers, but broken out by age bracket the picture is different: in the middle-age group, buyers earn more than non-buyers ($60,433 vs. $57,025). In the Adolescent and Old brackets, the relationship reverses — buyers actually earn *less* than non-buyers. Income is not a universal predictor; it reinforces purchase likelihood specifically within the highest-converting age group.

**Family size only matters at the high end.** Customers with 0–3 children all convert at a similar rate (47%–57%), showing no clear trend. But customers with 4 or more children convert much less often — 42.9% at 4 children, dropping sharply to 21.4% at 5 children — suggesting budget or priority constraints kick in once family size grows large, rather than family size mattering uniformly.

**Gender, education, and commute distance showed no meaningful effect.** Purchase rates were roughly flat across these dimensions, with no pattern strong enough to act on.

## Recommendation
Prioritize marketing spend toward **middle-age, higher-income customers with 3 or fewer children** — this segment shows both the highest and most consistent purchase propensity across every dimension tested. Deprioritize outreach to customers with 4+ children, where conversion likelihood drops sharply regardless of age or income.
