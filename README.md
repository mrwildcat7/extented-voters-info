# extented-voters-info
This repository serves as a guide for gathering additional information on addresses that voted on Gitcoin Grants during the Hacking On The Hackathon event and the OpenData Community. 

The notebook *extend_data.ipynb* outlines the guide and required data transformations. The queries folder contains the queries used in the notebook to generate the data, which are compatible with the Flipside Crypto platform.

The *queries* folder contains the queries utilized in the notebook to generate the data. These queries work with the flipsidecrypto platform.

The *results* folder has two files:
  * grant_votes_extended_v_01.csv
  
| Field | Description |
| :---- | :---------: |
| address | contributor/voter wallet |
| has_ens | indicates if a wallet has at least one Ethereum Name Service (ENS) associated |
| ens_count | number of ENS's associated with an address |
| has_defi_transactions | indicates if the wallet has interacted with a decentralized exchange (DEX) contract |
| count_defi_transactions | number of transactions made with DEX contracts |
| had_activity_before_december_2022 |	indicates if the wallet had activity before December 2022 |
| count_activity_before_december_2022 | number of transactions before December 2022 |
| had_activity_after_december_2022 | indicates if the wallet had activity after December 2022 |
| count_activity_after_december_2022 | number of transactions after December 2022 |
  
  * probably_sybils.csv: This file contains the same fields as the grant_votes_extended_v_01.csv file, but with filtered data, specifically addresses with low activity. The addresses with low activity are considered suspicious.
  
  contact
  
  discord: mrwildcat#1969
