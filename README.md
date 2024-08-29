# Streaming Effect: Analyzing the Causal Impact of Twitch Viewership on Active Player Engagement

This project investigates the causal relationship between Twitch viewership and active player engagement for popular online multiplayer games, using advanced time series analysis techniques. Our main objective is to understand how Twitch viewership impacts the number of active players in games like Rainbow Six Siege, Counter-Strike 2, and Rust.

## Table of Contents
- [Introduction](#introduction)
- [Data Collection](#data-collection)
- [Methodology](#methodology)
- [Models Used](#models-used)
- [Results](#results)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [Contributors](#contributors)
- [Acknowledgments](#acknowledgments)

## Introduction

The project aims to explore how Twitch viewership influences active player engagement. This analysis is crucial for gaming companies to strategize their marketing efforts and optimize player retention and acquisition through Twitch. Our primary case study is Tom Clancy’s Rainbow Six Siege, with comparisons to Counter-Strike 2 and Rust.

## Data Collection

Due to limited access to Twitch and Steam APIs, data was collected from two third-party sources, SteamDB and Sullygnome. These platforms provided daily metrics such as player counts, Twitch viewership statistics, and additional variables like game pricing, discounts, events, and tournaments, which were used to account for confounding factors.

## Methodology

### Data Preprocessing
- **Stationarity**: Applied Augmented Dickey-Fuller tests, first-differencing, and deseasonalization to ensure data stationarity.
- **Lag Analysis**: Created lagged variables to capture delayed effects between Twitch viewership and player engagement.

### Exploratory Data Analysis (EDA)
- Visualized trends and seasonality in player counts and Twitch viewership.
- Examined correlations to identify potential causal links.

## Models Used

1. **Linear Regression**: Initial model to identify basic associations between variables.
2. **Granger Causality Test**: Used to test the predictability of Twitch viewers on player counts.
3. **Causal Discovery Using Model Invariance (CDMI)**: A novel approach using knockoffs to identify causal links.
4. **Latent Peter and Clark Momentary Conditional Independence (LPCMCI)**: An advanced method to detect and estimate causal relationships in time series data, leveraging the TIGRAMITE library.

## Results

- **Rainbow Six Siege**: Found significant positive effects of Twitch viewership on player engagement with a lag of 1 to 14 days.
- **Counter-Strike 2**: Limited causal impact from Twitch viewership, likely due to its established player base predating Twitch.
- **Rust**: Identified positive causal links with a conversion ratio of up to 4% from Twitch viewership to active players.

## Recommendations

1. **Focus on Top Streamers and Tournaments**: For games like Rainbow Six Siege, collaborating with top streamers and organizing tournaments significantly boosts Twitch viewership and player engagement.
2. **Leverage Streaming Platforms as Feedback Channels**: Use insights from streamers and Twitch chat interactions to guide game updates and improve player satisfaction.
3. **Tailor Marketing Strategies**: Develop game-specific marketing strategies based on the causal impact of Twitch viewership observed.

## Limitations

- Lack of true experimental data to establish definitive causal relationships.
- Limited behavioral and demographic data on players and viewers.
- Model complexity and pruning in LPCMCI may affect causal effect estimations.

## Contributors

- **Chun Yat (Jeco) Cheung**
- **Yixuan (Ethan) Liu**
- **Yu (Sherry) Shi**

## Acknowledgments

Special thanks to Prof. Austin Pollok for guidance and support throughout this project.

---

This project was completed as part of the DSO 585 course at USC Marshall School of Business.
