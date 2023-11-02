# Addition-Financial-Competition-23-24
# Data Dictionary

## Branch Level Data

This dataset provides students with a count of transactions for every branch by transaction type as of the end of the month for the year 2022 until the end of July 2023. This data will enable students to analyze transaction patterns, identify popular services, and assess branch performance. This will aid in making data-driven decisions on future branch locations.

| **Column Names**            | **Data Type**   | **Description** |
|-----------------------------|-----------------|-----------------|
| EOM TRANS DATE              | datetime64[ns]  | End of Month Transaction Date |
| BranchCategory              | object         | AFCU Branch Location |
| ATM                         | int64          | Count of ATM (Automated Teller Machine) transactions for that month at that branch |
| Bill Payment                | int64          | Count of bill payment transactions for that month at that branch |
| Cash                        | int64          | Count of cash transactions for that month at that branch |
| Draft                       | int64          | Count of draft transactions for that month at that branch |
| ACH                         | int64          | Count of Automated Clearing House (ACH) transactions for that month at that branch |
| Fee                         | int64          | Count of fee-related transactions for that month at that branch |
| Credit/Debit Card           | int64          | Count of credit and debit card transactions for that month at that branch |
| Home Banking                | int64          | Count of home banking transactions for that month at that branch |
| Dividend                    | int64          | Count of dividend-related payout transactions for that month at that branch |

## Member Level Data

This dataset provides students with a count of transactions by transaction type for members as of the end of the month for the year 2022 until the end of July 2023. This data will enable students to analyze transaction patterns, identify popular services, and assess member transaction habits.

| **Column Names**            | **Data Type**   | **Description** |
|-----------------------------|-----------------|-----------------|
| Unique_Member_Identifier    | object         | Randomly generated number representative of Member Account Number |
| EOM TRANS DATE              | object         | End of Month Transaction Date |
| Age*                        | int64          | Member age based on age category (refer to the age category description table) |
| BranchCategory              | object         | Branch assigned based on Member's Address |
| address_zip                 | object         | Member's address Zip Code |
| n_accts                     | int64          | Number of accounts belonging to the member |
| n_checking_accts            | int64          | Number of checking accounts belonging to the member |
| n_savings_accts             | int64          | Number of savings accounts belonging to the member |
| n_open_loans                | int64          | Number of open loans belonging to the member |
| n_open_cd’s                 | int64          | Number of open Certificate of Deposits (CDs) belonging to the member |
| n_open_club_accts           | int64          | Number of open club accounts belonging to the member |
| n_open_credit_cards         | float64        | Number of open credit card accounts belonging to the member |
| ATMCount                    | int64          | Count of ATM transactions performed by the member during that month |
| BillPaymentCount            | int64          | Count of bill payment transactions performed by the member during that month |
| CashCount                   | int64          | Count of cash transactions performed by the member during that month |
| DraftCount                  | int64          | Count of draft transactions performed by the member during that month |
| ACHCount                    | int64          | Count of ACH transactions performed by the member during that month |
| FeeCount                    | int64          | Count of fee-related transactions accessed to the member during that month |
| Credit_DebitCount           | int64          | Count of credit/debit transactions performed by the member during that month |
| Home_Banking                | int64          | Count of home banking transactions performed by the member during that month |
| WireCount                   | int64          | Count of wire transfer transactions performed by the member during that month |
| DividendCount               | int64          | Count of dividends paid out to the member during that month |