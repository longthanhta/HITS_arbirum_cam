# HITS-based Scam Detection in Arbitrum Airdrop

## Overview
This project utilizes the Hyperlink-Induced Topic Search (HITS) algorithm to identify scam accounts on Twitter during the Arbitrum airdrop. The methodology is based on the concept that legitimate sources (authorities) are referenced by reliable hubs, while scam networks create fake hubs to amplify fraudulent authority links.

## How It Works
- The scam detection approach leverages the HITS algorithm to analyze Twitter network connections.
- Scammers create fake Arbitrum accounts and use bot networks to amplify these fraudulent links.
- The project identifies these patterns and highlights the most influential scam accounts.

## Data Source
Data can be downloaded from the [Osome Network Analysis Tool](https://osome.iu.edu/tools/networks/) using the following parameters:
- **Hashtags:** `#ARB, #Airdrop, #Arbitrum`
- **Network Type:** Retweet network (rq)
- **Date Range:** March 16, 2023 - March 30, 2023

Save the dataset as `Twitter_ARB_Airdrop_Arbitrum_Osome.csv`.

## Dependencies
Ensure you have the following Python libraries installed:
```bash
pip install pandas networkx pyvis beautifulsoup4 tqdm numpy
```

## Usage
1. Load the dataset in the script:
   ```python
   file_path = 'Twitter_ARB_Airdrop_Arbitrum_Osome.csv'
   ```
2. Run the notebook to process and analyze the data.
3. The visualization will help identify scam hubs and authorities.

## Visualization
The project generates a network graph using **NetworkX** and **Pyvis** to display scam account connections.

## Results
The output includes:
- Identification of high-authority scam accounts.
- Network visualization to illustrate fraudulent amplification.

## Future Improvements
- Enhance filtering techniques to refine scam detection.
- Integrate real-time monitoring for scam detection.

## Author
This project was developed by `longthanhta` to analyze scam activity in the Arbitrum ecosystem.

