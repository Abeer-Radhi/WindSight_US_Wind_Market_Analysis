# WindSight: US Wind Market Entry Strategy

**Where are the strongest aging fleet opportunities in the U.S. wind market?**

U.S. wind turbine fleet analysis | Group Data Analytics Project, General Assembly (DAB 26)

## Overview

As WOW! evaluates entry into the U.S. wind market, this project examines the age, location, rated capacity, and reported operators of the observed turbine fleet to identify areas worth further repowering assessment.

The analysis uses 2022 as the reference year for turbine age. Turbines aged 20 years or more are treated as the aging fleet segment for screening purposes.

**Audience:** Wind energy companies evaluating market entry, repowering opportunities, and operator outreach.

## Key Findings

- Of 70,195 turbines with a recorded commissioning year, **6,252 (8.9%) were at least 20 years old as of 2022**.
- **Median turbine rated capacity increased from 1.80 MW in 2011 to 2.82 MW in 2021**, a 56.7% increase.
- **California had the largest aging fleet**, with 3,417 turbines aged 20 or more.
- **Texas followed with 894 aging turbines**, representing approximately 927 MW of rated capacity.
- Among matched operator records, **Terra-Gen had the largest aging fleet**, followed by Allete Clean Energy and FPL Energy Vansycle.
- Operator records were matched to **80.6% of turbines aged 20+**, so operator results represent the matched portion of the aging fleet.

## Recommendations

1. **Geographic Focus:** Prioritize California (3,417 aging turbines), followed by Texas (894 aging turbines, 927 MW).
2. **Operator Outreach:** Start with Terra-Gen, followed by Allete Clean Energy and FPL Energy Vansycle.
3. **Repowering Assessment:** Evaluate aging sites for replacement with newer, higher-capacity turbine models.

## Data

| Dataset                    | Provides                                                                            |
| -------------------------- | ----------------------------------------------------------------------------------- |
| U.S. Wind Turbine Database | Turbine location, commissioning year, rated capacity, project and state information |
| EIA 923 Wind Data          | Plant and reported operator information used for operator matching                  |

The cleaned datasets used in the analysis are included in the `datasets/` folder. The analysis is based on 70,195 turbines with a valid commissioning year.

## Method

1. **Clean and validate:** Prepared the wind turbine and EIA 923 datasets and checked key identifiers, dates, and capacity fields.
2. **Profile fleet age:** Calculated turbine age as of 2022 and identified turbines aged 20 years or more.
3. **Analyze capacity:** Examined median turbine rated capacity across commissioning years and compared 2011 with 2021.
4. **Match operators:** Linked aging turbines to EIA 923 operator records and measured match coverage before ranking operators.
5. **Assess geography:** Compared aging turbine counts by state to identify the largest concentrations.
6. **Visualize:** Built the final charts in Python so the presentation results can be reproduced directly from the analysis notebook.

## Tools

`Python` (pandas, matplotlib) · `Jupyter Notebook`

## Repo Contents

```text
WindSight-US-Wind-Market-Analysis/
├── README.md
├── datasets/
│   ├── Wind_Turbine_Cleaned.csv
│   └── EIA923_2020_Wind_Cleaned.csv
├── notebooks/
│   ├── Wind_Turbine_Data_Cleaning.ipynb
│   ├── EIA923_Data_Cleaning.ipynb
│   └── WindSight_Analysis.ipynb
└── presentation/
    └── US_Wind_Market_Entry_Strategy.pdf
```

## Limitations

- The 20-year threshold is used as an analytical screening point and does not mean every turbine aged 20+ has reached the end of its operating life.
- Rated capacity is nameplate capacity, not actual electricity generation, efficiency, reliability, or financial return.
- EIA 923 identifies reported operators, not necessarily legal asset owners.
- Operator matching covered 80.6% of turbines aged 20+, so operator rankings do not represent the full aging fleet.
- Repowering decisions would require additional site-level, technical, generation, cost, and financial analysis.

---

**Abeer Radhi** · LinkedIn: [www.linkedin.com/in/abeerradhi](https://www.linkedin.com/in/abeerradhi/)
