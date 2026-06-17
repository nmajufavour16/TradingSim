# Trading Simulation Engine
Core Idea:
To build a virtual stock market where users can buy and sell assets using simulated money.

The goal is not predicting stock prices but managing transactions correctly.

> *Features*
1. *User Account*
When the program starts:
Balance: $100,000

Users can:
1. View Market
2. Buy Asset
3. Sell Asset
4. View Portfolio
5. Transaction History
6. Exit

2. *Market Data*
You can create assets such as:
GOLD
OIL
APPLE
TESLA
BITCOIN

Each asset has:
Name
Price
Available Quantity

Example:
GOLD = $200
OIL = $50
TESLA = $300
Transaction Validation

Before buying:
Check:

Does asset exist?
Does user have enough money?
Is quantity valid?

Example:
Buy 10 TESLA

Cost:
10 × 300 = 3000
If balance:
2500
Reject transaction.

> Selling Validation
Check:

Does user own asset?
Does user own enough quantity?

Example:
Own: 5 GOLD
Attempt: Sell 8 GOLD
Reject.

> Portfolio Management

Track:
Asset
Quantity
Average Buy Price
Current Price
Profit/Loss

Example:

TESLA
Owned: 20
Bought At: 250
Current: 300

Profit:
20 × (300 - 250)
Transaction History

Store:
Date
Action
Asset
Quantity
Price

Example:
BUY TESLA 10 @ 300
SELL GOLD 5 @ 210