# BayesianStats Project
### Which measures are most effective in attenuating a coronavirus outbreak?

Samples:
- Top X countries with available information
- Broken down into weeks
- Exclude isolated cases, start from 2nd consecutive week of Growth
- Exclude isolated cases, start from evidence of community spread

Response variable:
- Growth rate per week


Independent variables (measures imposed):
- Airport screening (temperature)
- Travel Advisories (not ban) [binary]
- Number of countries banned from entering [count]
- Number of countries banned from travel [count]
- Mandatory 14-day quarantine from countries [none, partial, total]
- School closure [none, partial, total]
- Lockdown [none, partial, total]
- Hand-wash/ hygiene campaign [binary]
- Religious gathering shutdown [none, partial total]


Random Variable:
- Random effect of country

Model(s):
- Bayesian regression (mixed effects)

Considerations:
- Since measures will inherently have a time lag between start and a decrease in cases: should have a time delay
  - match measures to outcomes after 2 weeks
  - match measures to outcomes after modelled mean (or median) recovery period
    - where to get data?
  - Disease in 2 phases, imported cases and community spread, these may have vastly different growth rates
    - need to check assumption


