# blockchain-fraud-analysis-case-001
This case study explores the forensic tracing of a suspicious on-chain transaction on Ethereum involving a $24,000+ USDT transfer. Leveraging tools like Etherscan, the transaction path, wallet behaviour, and potential risk indicators were analysed.
0x1ec15d970d777395bc331785d9f81feca8111377cc87b21a60178a7ae1e4a418
📍 Transaction Details:
- **Value:** $24,363.09 USDT
- **From:** 0x18E29605...7A73872F6
- **To:** 0x499d2906...D0A001e6d
- **Date:** 21 July 2025
- **Status:** Confirmed
- **Gas:** 90,000 (46,109 used)

## Red Flags:
- Sudden high-value transfer from an address with no prior outgoing activity.
- Use of common token hopping pattern (ETH → USDT).
- No smart contract interaction other than direct transfer.
- Possible early-stage layering (potential laundering).

## Screenshots:
Stored in the `/screenshots` folder (blurred for privacy).

## Analyst Note:
This repo is part of a broader initiative to highlight behavioral patterns in blockchain fraud for the purpose of improving forensic practices and platform security.


<img width="1841" height="707" alt="image" src="https://github.com/user-attachments/assets/bcbf2aad-cff4-47e0-82e1-9ce7cfe554ba" />
<img width="1803" height="398" alt="image" src="https://github.com/user-attachments/assets/79cff8fe-389c-47ca-bf40-d35e032b8a1a" /> 
<img width="1833" height="503" alt="image" src="https://github.com/user-attachments/assets/ee5a234e-2612-4d54-9e21-15d009f8bba2" /> In this screenshot, we can see that the wallet which received the USDT has not made an outgoing transfer in over a year — reducing the likelihood that this is an actively used wallet. Typically in crypto fraud, cold wallets are used for the extraction and short-term holding of stolen funds. These wallets are often “warmed up” for a few weeks or months in advance to avoid triggering anti-fraud signals. Fraudsters intentionally keep them dormant until ready, minimizing detection risks while executing high-value transfers.


<img width="1791" height="218" alt="image" src="https://github.com/user-attachments/assets/48d7e7d5-1e08-4d0e-a65e-10759ef97b86" /> Here we have a collection of the receiving wallets most recent outgoings. We will now trace the blockchain activity of the most recent transfer for any further cold wallet signs 
<img width="1807" height="485" alt="image" src="https://github.com/user-attachments/assets/7af37a40-3a30-444c-b23f-eabe1ae5eb3d" /> here we can see the transaction was a transfer of 'DAI' token to another 'DAI' wallet . 
<img width="1789" height="692" alt="image" src="https://github.com/user-attachments/assets/1ecf29c4-9126-48c4-b28d-dc3e6ee32f13" /> Here we can see the wallet it was transferred into and we can see that the wallet in question hasn't had activity in over a year and there is transactions to known centralised exchanges e.g kucoin, uniswap etc. Reducing the likelihood this is a cold wallet or this transfer was part of a wider mixing of the funds.










