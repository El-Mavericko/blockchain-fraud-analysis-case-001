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
<img width="1833" height="503" alt="image" src="https://github.com/user-attachments/assets/ee5a234e-2612-4d54-9e21-15d009f8bba2" /> In this screenshot we can see that the wallet that received the USDT, hasn't made an outgoing transfer in over a year, which reduces the likelihood that this is fraud. Furthemore typically seen in crypto fraud cold wallets used for extraction and holding of stolen funds tend to be fresh or warmed up for a couple weeks or months in advance. The fraudsters do this to avoid raising detection whilst submitting the network requests.



