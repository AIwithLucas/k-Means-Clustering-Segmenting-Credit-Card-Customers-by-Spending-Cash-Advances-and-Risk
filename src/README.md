# Credit Card Dataset for Clustering

## Dataset Description

Exploratory analysis and clustering algorithm to identify customer segments

## Segmentation Focus (k-Means Clustering)

    1. High Spenders: Customers with high purchases / frequent transactions

    2. Cash-Heavy Users: Customers relying heavily on cash advances (indicative of potential financial stress)

    3. Low Risk Customers: Customers paying balances in full / maintaining low balances

    4. Installment Purchaser: Customers preferring payment flexibility (ideal for targetting marketing)

## Features of the Dataset

- Number of records: 30,000
- Number of features: 23

| **Feature Name**          | **Data Type** | **Description**                                             |
| ------------------------- | ------------- | ----------------------------------------------------------- |
| `ID`                      | Integer       | Unique identifier for each customer.                        |
| `Balance`                 | Float         | Total balance on the credit card account.                   |
| `BalanceFrequency`        | Float         | Frequency of balance updates in a given time period.        |
| `Purchases`               | Float         | Total monetary value of all purchases made by the customer. |
| `OneOffPurchases`         | Float         | Value of single high-value purchases.                       |
| `InstallmentsPurchases`   | Float         | Value of purchases made in installments.                    |
| `CashAdvance`             | Float         | Total value of cash advances taken by the customer.         |
| `PurchaseFrequency`       | Float         | Proportion of months with at least one purchase.            |
| `OneOffPurchaseFrequency` | Float         | Proportion of months with at least one one-off purchase.    |
| `InstallmentFrequency`    | Float         | Proportion of months with installment purchases.            |
| `CashAdvanceFrequency`    | Float         | Proportion of months with cash advances.                    |
| `CashAdvanceTrx`          | Integer       | Number of cash advance transactions.                        |
| `PurchasesTrx`            | Integer       | Number of purchase transactions.                            |
| `CreditLimit`             | Float         | Maximum credit limit of the card.                           |
| `Payments`                | Float         | Total payments made by the customer.                        |
| `MinimumPayments`         | Float         | Minimum payments required for the account.                  |
| `PRCFullPayment`          | Float         | Ratio of months with full payment of balance.               |
| `Tenure`                  | Integer       | Number of months the customer has been with the bank.       |

## Features to be segmented

| **Feature Name**                     | **Segmentation Description**                                                                                                                                 |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Balance**                          | Clustering based on total balance can help group customers by their spending or debt levels.                                                                 |
| **Purchases & Purchase Frequencies** | These features can identify customers who frequently use their credit cards versus those who use them occasionally.                                          |
| **Cash Advances**                    | Customers who frequently request cash advances can be clustered separately for targeted marketing strategies.                                                |
| **Payments**                         | Analyzing customers based on payment behaviors may reveal those who are more diligent in repaying versus those who make irregular payments.                  |
| **Credit Limit**                     | Segments can be formed based on credit limit utilization, grouping those with high utilization from those who maintain low balances relative to their limit. |
| **Tenure**                           | Customers with different account ages might cluster into different groups depending on how long they have been using the service.                            |
