# Global Health Spending

**Who pays for health care, what do they pay for, and does it show up in how long people live?**

A team data analysis of country-level health expenditure from 2000 to 2023, broken down by who pays (government, private insurance, out-of-pocket, external aid) and what the money is spent on (curative care, long-term care, prevention, and so on). We merged in outside data on life expectancy, GDP per capita, population, and World Bank-style income groups to see how spending patterns line up with wealth and health outcomes.

**Team:** Rena, Coco, Ibrahim, Matthew, Yihan

---

## Questions we asked

1. **Who pays?** How does the split between government, voluntary insurance, out-of-pocket, and external financing change with national income?
2. **When the citizen pays.** How heavy is the out-of-pocket burden, and how has the state-versus-citizen balance shifted over 20 years?
3. **Where does the money go?** How do countries divide spending across curative care, long-term care, medical goods, and prevention, and does that relate to life expectancy?

## Data

| Source | What we used it for |
|---|---|
| Health expenditure by **financing scheme** | Who pays (government and compulsory, voluntary insurance, out-of-pocket, external) |
| Health expenditure by **spending purpose** | Where the money goes (curative, rehabilitative, long-term, ancillary, medical goods, preventive, governance, other) |
| Life expectancy | Outcome variable |
| GDP per capita | Wealth control and comparison |
| Population | Bubble sizes in plots |
| Income group classification | Low / lower-middle / upper-middle / high income grouping |

## Key findings

**Who pays**
- The share of health spending coming from government and compulsory schemes rises with income: about 33% (low), 45% (lower-middle), 56% (upper-middle), 71% (high). The biggest jump is from low to lower-middle income.
- Even in high-income countries, roughly 30% of funding comes from somewhere other than government.
- Over 20 years, high- and upper-middle-income countries stayed government-heavy, while low-income countries stayed more reliant on out-of-pocket payments than on government funding.

**When the citizen pays**
- Wealthier countries have both higher government spending per person and higher out-of-pocket spending per person, so the *share* is what separates rich and poor systems, not the raw amount.
- Countries that rely heavily on out-of-pocket financing tend to have lower life expectancy. Many Sub-Saharan African countries sit in that corner of the plot; most European countries and the US sit at low reliance and high life expectancy.

**Where the money goes**
- Spending mix is fairly similar across income groups, but preventive care and governance shrink as a share of spending in wealthier countries while long-term care and rehabilitation grow.
- Looking at *share* alone is misleading: two countries can devote the same percentage to prevention and spend wildly different dollars per person.
- Looking at *dollars per person*, higher preventive spending goes with longer life expectancy (quadratic fit, R² = 0.41).
- Total health spending per capita is strongly associated with life expectancy (quadratic fit, R² = 0.79), with diminishing returns at high spending levels.

## Limitations

- **Associations, not causation.** Income drives both spending and life expectancy, so a lot of the relationships above are likely confounded by wealth. We did not control for this in the plots.
- **Share vs. per-capita can point in opposite directions.** Countries with a high preventive *share* tend to have lower life expectancy, mostly because they are low-income countries with little total money. Per-capita prevention spending shows the opposite pattern.
- **Group averages hide spread.** Income-group means are unweighted by population.
- **Not-classified countries** (no income group) are noisy and are mostly left out of the comparisons.
- Quadratic fits are descriptive. In the prevention model the log-spending term alone was not significant (p = 0.49); the curvature term drives the fit.

## My Contributions:

Created visualizations and explored data about finance scheming and spending.

## Contributors

Rena, Coco, Ibrahim, Matthew, Yihan

