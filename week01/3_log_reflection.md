# 3. AI Use Log and Reflection

## AI-use log

| AI use / suggestion | Verification against the dataset | Decision |
|---|---|---|
| Suggested testing whether the average recorded price changes across dates. | The CSV contains `date` and numeric `price`, so a daily mean can be calculated. | **Accepted with limits:** this is a simple unweighted mean, not a formal inflation index. |
| Suggested identifying which item has the greatest price variation. | The CSV contains `item` and numeric `price`; standard deviation can be calculated by item. | **Accepted:** the calculation is supported by the available columns. |
| Suggested analyzing corn prices. | The item labels are `Staple A`, `Oil B`, `Pulse C`, and `Sweetener D`; there is no corn item. | **Rejected:** the dataset does not identify corn. |
| Suggested linking food prices with fuel prices or explaining causes of price changes. | There is no fuel, tax, supply-chain, or policy variable in the CSV. | **Rejected:** those questions cannot be tested with this dataset. |

## What the data can and cannot say

The dataset can show the recorded prices of four illustrative items in two anonymized cities over twelve dates. It can be used to calculate averages, compare items, and measure variation across the observed period. It cannot establish the actual prices paid by households, represent the whole Pakistani market, or explain why prices changed. The file explicitly labels its records as illustrative teaching data rather than actual PBS observations.


Use this as a factual checklist when writing your own reflection:
- Which of your original claims became measurable questions?
- Which AI suggestion did you accept, and why?
- Which suggestions did you reject because the required variable was missing?
- What did you learn about the difference between a pattern and an explanation?
- How did checking the data dictionary change your thinking?



## Verification record

Before submission, run the notebook and confirm that the displayed row count, item count, date count, calculations, and charts match the CSV. Record any changes you make after checking.
