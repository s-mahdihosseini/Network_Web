# Dataset for: The Global Network of Liquidity Lines

- [Draft, coming soon!](https://personal.lse.ac.uk/reisr/papers/99-infdis.pdf)

![Description of the image](Map_Network.png)


## Authors:

- [Saleem Bahaj](https://sites.google.com/site/saleembahaj/home)
- [Marie Fuchs](https://www.lse.ac.uk/economics/people/research-students/marie-fuchs)
- [Ricardo Reis](https://www.r2rsquared.com/)

## Date:

April 2024

## Summary
- A central bank cross-border liquidity line is an agreement between two central banks to
provide a collateralised loan of currency from one to the other. They have been around for
a long time, but have risen in prominence over the last twenty years. Following both the
great financial crisis and the pandemic, central banks expanded the number of lines and
relied on them to restore financial stability. By 2023, the funds committed to the liquidity
lines were well above the lending capacity of the International Monetary Fund (IMF). 

- These agreements are varied in their signatories and in their characteristics. For instance, while swap lines get most of the attention, there are many repurchase agreements
as well. Also, while borrowing from a line usually means money issuance by one of the
central banks, there are some large lines that instead lend out existing USD central bank
reserves. Finally, the People’s Bank of China (PBoC) has many bilateral lines, while the
Federal Reserve (Fed)’s lines are concentrated in one large multilateral arrangement, and
the European Central Bank (ECB) has a mix in between.

- This paper provides a comprehensive dataset of central bank cross-border liquidity
lines at the agreement level: by date and duration (2000-23), by source currency (USD,
EUR, RMB, others), by type (bilateral or multilateral), by funding structure (pooled or
by individual bank), by counterparties (central banks), and by some terms (like the collateral). This dataset was collated from public sources, and is **freely available for other
researchers to use**. We use these data to establish three novel sets of facts.


## Dataset
| Column               | Description                                              | 
|----------------------|----------------------------------------------------------| 
| deal_ID              | Unique ID for each row representing a deal               | 
| deal_type            | String indicating reciprocity type                                                                  | 
| framework            | String indicating if deal is part of larger framework agreement                                      | 
| reciprocal_deal     | If deal is reciprocal, numeric value indicating matching reciprocal deal                             | 
| collaterepoal       | String indicating type of collateral underlying each deal                                           | 
| ISO_source           | Source country ISO 3166-1 (alpha-3) country code                                                    | 
| source_country      | Source country name                                                                                | 
| ISO_recipient       | Recipient country ISO 3166-1 (alpha-3) country code                                                 | 
| recipient_country   | Recipient country name                                                                             | 
| start_date           | Agreement signature date or press release date                                                      | 
| end_date             | Agreed expiration date as mentioned in press release                                                | 
| existence_previous_deal | Indicator variable for whether a deal of any kind existed between the two countries in the past | 
| deal_action         | String variable indicating the role of each deal within a deal chain                                 | 
| previous_deal       | (Backward-looking) if deal_action renew or reactivate, previous_deal indicates prior deal of identical characteristics being renewed or reactivated | 
| currency_of_deal    | Agreed currency of the deal (ISO4217 standard abbreviation)                                          | 
| source_currency     | Source central bank currency (ISO4217 standard abbreviation)                                         | 
| source_currency_deal | Dummy variable                                                                                     | 
| deal_currency_amount | Quoted maximum amount agreed on in currency of the deal; registered in billion as mentioned in press release | 
| USD_amount          | If deal amount mentioned in USD in press release, then USD maximum amount, otherwise NA            | 
| unlimited           | Indicator variable for whether deal amount was unlimited                                             | 
| initiative          | Initiative under which deal was agreed (if any)                                                      | 

For more detailed analysis and data, here is a link to the dataset: 
## Updates

This research is updated regularly to reflect the latest data and analysis.

## Acknowledgment

We thank Marina Feliciano, and other people who helped!

---

*This website is for test purposes for Ricardo and the team.*
