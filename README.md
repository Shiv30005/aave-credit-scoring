# Aave V2 Wallet Credit Scoring

## Methodology
1. Load transaction data from JSON
2. Extract key features:
   - Deposit/borrow/repay amounts
   - Liquidation events
   - Transaction frequency
   - Account activity duration
3. Calculate raw scores using weighted rules:
   - Positive weights for deposits and repayments
   - Negative weights for liquidations
4. Normalize scores to 0-1000 range
5. Output CSV with wallet addresses and scores

## Usage
Run script with input JSON path:
`python score_wallets.py input.json`