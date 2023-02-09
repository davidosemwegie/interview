# Affiniti Engineering Interview

Feel free to use any language or framework you are comfortable with. We are not looking for a perfect solution, but we are looking for a solution that is well thought out. Feel free to use any resources you need to complete the challenge.

**All currency outputs should be in USD format ($xxx,xxx,xxx.xx)**

## Part A

The file `transactions.json` contains an array of financial transactions provided as an API response from a user's bank. A transaction `type` can be either: `Deposit`, `Withdrawal`, `Interest Payout`, or `Internal Transfer`. Some transactions may incur fees.

1. In the most efficient way possible, write a function that takes in the array of transactions and returns the sum of all `amounts` that was transacted. Fees can be ignored.
2. Write a function that, when given a transaction `type`, returns the total amount of money that was transacted for that type in this array. For example, if the `type` is `Deposit`, the function should return the total amount of money for transactions with the `Deposit` type.
3. Write a function that returns the count of each transaction type.

## Part B

The above user's bank have realized that developers interacting with their API had it too easy. They have opted to change their API responses to CSV format. The file `transactions.csv` contains the same data as `transactions.json`, but in CSV format.

1. Write a function that takes in the CSV file and returns the total volume of money that was transacted. Fees can be ignored.
2. Assuming that this transaction data is the entire history of the user's account, write a function that returns the current balance of the account. You can assume that `Deposit` & `Interest Payout` transactions are always positive, `Internal Transfer` transactions do not change the balance, and `Withdrawal` transactions are always negative.