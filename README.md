# Streaming Influence: Analyzing the Causal Impact of Twitch Viewership on Active Player Engagement
## Description
This project aims to analyze the causal relationship between a game’s Twitch viewership and its active player engagement, using Tom Clancy’s Rainbow Six Siege as the primary case study. The analysis extends to other popular online multiplayer shooting games, such as Counter-Strike 2 and Rust.

In February 2024, Ubisoft's Six Invitational 2024 event set a record for the highest peak Twitch viewership, which was followed by a significant increase in the average player count for Rainbow Six Siege. This observation led to the hypothesis that Twitch viewership can influence player engagement, providing valuable insights for gaming companies to refine their marketing strategies.

**Key Highlights:**

**Objective:** Investigate how Twitch viewership impacts active player engagement.

**Games Analyzed:** Tom Clancy’s Rainbow Six Siege, Counter-Strike 2, and Rust.

**Methodologies:** Linear Regression, Granger Causality Test, Causal Discovery Using Model Invariance (CDMI), and Latent Peter and Clark Momentary Conditional Independence (LPCMCI).

**Data Sources:** Data was gathered from third-party websites, SteamDB and Sullygnome, due to limited access to historical data from official Twitch and Steam APIs.

**Findings:** The analysis suggests a causal relationship between increased Twitch viewership and higher player engagement, with varying time delays depending on the game.

This project provides a framework for understanding the influence of live-streaming platforms on gaming communities, offering actionable recommendations for game developers and marketers to enhance player engagement through strategic Twitch collaborations.

Please see [DSO 585 Project Presentation-compressed.pdf](https://github.com/sputnik-h/Twitch-x-Steam/blob/main/DSO%20585%20Project%20Presentation-compressed.pdf) and [DSO 585 Team 2 Final Report.pdf](https://github.com/sputnik-h/Twitch-x-Steam/blob/main/DSO%20585%20Team%202%20Final%20Report.pdf) for further details about the project

## Environment Setup (for CDMI) and Installaion 

Causal Discovery Using Model Invariance (CDMI) in the project is based on research by [Wasim Ahmad, Maha Shadaydeh, and Joachim Denzler from the Friedrich Schiller University Jena](https://arxiv.org/pdf/2207.04055).

To setup the environment used in this project:

1. Download and unzip cdmi-main.rar
2. Install dependencies: `pip install -r requirements.txt` (Python Version 3.11.7)
3. Set up environment variables if necessary.

## Other Contributors

- **[Jeco (Chun Yat) Cheung](https://www.linkedin.com/in/jecocheung/)** 
- **[Yu (Sherry) Shi](https://www.linkedin.com/in/sherryshi91/)** 
