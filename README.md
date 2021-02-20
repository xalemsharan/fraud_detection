# Fraud Detection Model

Fraud is a very rare event, approximately only 1 in 1,000 transactions is a fraudulent. Identifying fraudulent transactions could be challenging due to its highly rare nature.

This project aims at helping financial institutions in identifying fraudulent transactions and prevent/minimize financial loss.

**Where does fraud happen?**
* Fraud is observed in Cash Out and Transfer type transactions only.
* Also, fraud is observed in Customer 2 Customer transactions only.

**When does fraud happend?**
* Majority of fraudulent transactions happen during night.
* Fraudulent transactions peak between 3am and 6am, and goes as high as 58% of transactions.
* Less than 1% of transactions during day are fraudulent.

**Characteristics of fraudulent transaction amount:**
* Proportion of fraudulent transactions in case of transaction amount ending in 0 is little higher than rest of the digits.
* Human beings tend to come up with round numbers when they make-up numbers.

**Cues to identify fraudulent transactions:**
* Proportion of fraudulent transactions in case of transaction amount ending in 0 is little higher than rest of the digits.
* Human beings tend to come up with round numbers when they make-up numbers.

**Important features for fraud detection model:**
* `zeroBalanceDest`: Whether the destination account balance amount after the transaction was zero.
* `ln_errorBalanceOrig`: Log of error in the origin account balance amount after the transaction.
* `transactionPeriod_Peak`: Whether the transaction was made during peak fraudulent transaction period (midnight).
