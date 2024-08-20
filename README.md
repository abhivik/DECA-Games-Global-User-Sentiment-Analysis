# DECA Games Community Sentiment and Feedback Analysis for Game KPI Improvement

## Project Overview

This project is focused on analyzing user reviews for various games developed by DECA Games. The primary objective is to understand community sentiment, identify key factors affecting player satisfaction, and correlate these insights with game KPIs to provide actionable recommendations for improvement. This analysis was conducted to demonstrate data analysis skills and support an application for the Junior Data Analyst position at DECA Games.

## Project Goals

- **Sentiment Analysis**: To gauge player sentiment towards DECA Games' titles across multiple countries.
- **Game KPI Improvement**: To identify key areas impacting player satisfaction and suggest improvements.
- **Visualization and Reporting**: To present insights using Tableau to make data-driven recommendations actionable and understandable.

## Steps Taken

### 1. Selection of Games
Thirteen popular games developed by DECA Games were selected for user sentiment analysis. These games include:

- **The Walking Dead: No Man's Land** [Google Play Store](https://play.google.com/store/apps/details?id=com.nextgames.android.twd) | [App Store](https://apps.apple.com/us/app/the-walking-dead-no-mans-land/id970417047)
- **Dead Trigger 2** [Google Play Store](https://play.google.com/store/apps/details?id=com.madfingergames.deadtrigger2) | [App Store](https://apps.apple.com/us/app/dead-trigger-2-zombie-games/id720063540)
- **Shadowgun Legends** [Google Play Store](https://play.google.com/store/apps/details?id=com.madfingergames.legends) | [App Store](https://apps.apple.com/gb/app/shadowgun-legends-online-fps/id1091251242)
- **Dead Trigger** [Google Play Store](https://play.google.com/store/apps/details?id=com.madfingergames.deadtrigger) | [App Store](https://apps.apple.com/us/app/dead-trigger-survival-shooter/id533079551)
- **Samurai II: Vengeance** [Google Play Store](https://play.google.com/store/apps/details?id=com.madfingergames.SamuraiIIAll) | [App Store](https://apps.apple.com/us/app/samurai-2-vengeance/id392486160)
- **Celtic Heroes** [Google Play Store](https://play.google.com/store/apps/details?id=com.onethumbmobile.celticheroes) | [App Store](https://apps.apple.com/us/app/celtic-heroes-mobile-mmorpg/id431837446)
- **Unkilled** [Google Play Store](https://play.google.com/store/apps/details?id=com.madfingergames.unkilled) | [App Store](https://apps.apple.com/us/app/unkilled-zombie-online-fps/id969488951)
- **Call me a Legend** [Google Play Store](https://play.google.com/store/apps/details?id=com.sixwaves.cml&hl=en&gl=US) | [App Store](https://apps.apple.com/us/app/call-me-a-legend/id1449121741)
- **Call me a Gangsta** [Google Play Store](https://play.google.com/store/apps/details?id=com.empirestudiosinc.cmg&hl=en&gl=US) | [App Store](https://apps.apple.com/us/app/call-me-a-gangsta/id1530493373)
- **Robbery Bob** [Google Play Store](https://play.google.com/store/apps/details?id=com.chillingo.robberybobfree.android.row) | [App Store](https://apps.apple.com/us/app/robbery-bob-king-of-sneak/id503869041)
- **Robbery Bob 2** [Google Play Store](https://play.google.com/store/apps/details?id=com.chillingo.robberybob2.android.gplay) | [App Store](https://apps.apple.com/us/app/robbery-bob-2-comic-thief/id974514406)
- **Gods and Glory** [Google Play Store](https://play.google.com/store/apps/details?id=com.fridaysgames.godsandglory) | [App Store](https://apps.apple.com/us/app/gods-and-glory-war-of-thrones/id1050101469)
- **DragonVale** [Google Play Store](https://play.google.com/store/apps/details?id=com.backflipstudios.android.dragonvale) | [App Store](https://apps.apple.com/us/app/dragonvale/id440045374)



### 2. Geographic Scope
A total of 23 countries were chosen to ensure a comprehensive analysis, representing different regions:

- United States, United Kingdom, Germany, France, Italy, Spain, Russia, Japan, South Korea, India, China, Singapore, United Arab Emirates, Canada, Australia, Brazil, Mexico, South Africa, New Zealand, Turkey, Vietnam, Poland, Netherlands.

### 3. Data Collection
#### Google Play Store:
The `google_play_scraper` Python library was used to scrape user reviews from the Google Play Store, focusing on game name, country, review content, rating, and date of review. Sentiment analysis was conducted using the VADER sentiment analysis tool.
- [Google Play Store Scraper Script](https://github.com/abhivik/DECA-Games-Global-User-Sentiment-Analysis/blob/main/google_store_scrapper.ipynb)
- [Processed Data](https://github.com/abhivik/DECA-Games-Global-User-Sentiment-Analysis/blob/main/google_store_processed.csv)

#### Apple App Store:
Similarly, the `app_store_scraper` Python library was used to gather and process reviews from the Apple App Store.
- [Apple App Store Scraper Script](https://github.com/abhivik/DECA-Games-Global-User-Sentiment-Analysis/blob/main/Apple_Store_scrapper.ipynb)
- [Processed Data](https://github.com/abhivik/DECA-Games-Global-User-Sentiment-Analysis/blob/main/apple_store_processed.csv)

### 4. Data Processing
After scraping data from both stores, the datasets were combined and cleaned for further analysis. This included removing duplicates, handling missing values, and ensuring consistency across the datasets.
- [Combined and Processed Data Script](https://github.com/abhivik/DECA-Games-Global-User-Sentiment-Analysis/blob/main/Combined%20processed.ipynb)
- [Final Combined Data](https://github.com/abhivik/DECA-Games-Global-User-Sentiment-Analysis/blob/main/combined_sentiment_review_data.csv)

### 5. Data Analysis and Visualization
Tableau was used to visualize the results, focusing on the following key areas:

- **Overall Game Ratings (Bar Chart)**: Provides an overview of average ratings for each game.
- **Geographical Rating Analysis (Heat Map)**: Illustrates average ratings by country, highlighting geographic trends in user satisfaction.
- **Review Trends Over Time (Line Chart)**: Tracks the volume of reviews over time to detect patterns and spikes in user activity.
- **Sentiment Trends Over Time (Stacked Line Chart)**: Shows how user sentiment has evolved over time for different games.
- **Sentiment Distribution by Game (Bar Chart)**: Compares the distribution of positive, neutral, and negative sentiments across different games.
- **Negative Sentiment Analysis (Text Tables)**: Focuses on reviews with negative sentiment to identify common issues and areas for improvement.

The visualizations can be explored in detail on the Tableau Public dashboard:
- [Tableau Dashboard](https://public.tableau.com/app/profile/abhivik/viz/DECAGamesGlobalUserSentimentAnalysisDashboard/DCEAGamesGlobalUserSentimentAnalysis?publish=yes)

![DCEA Games Global User Sentiment Analysis](https://github.com/user-attachments/assets/17732799-d49f-4685-abac-70c5f6d3ef14)

## Conclusion
The analysis provides valuable insights into how DECA Games' titles are perceived by players across different regions. By identifying patterns in user sentiment and feedback, informed recommendations can be made to enhance player satisfaction and engagement.

## Future Work
- Extending the analysis to include more games and countries.
- Incorporating additional data sources, such as social media sentiment analysis, for a more comprehensive view of user feedback.
- Exploring advanced machine learning techniques for sentiment analysis to improve the accuracy and depth of insights.

## Contact
For any inquiries or further discussion about this project, feel free to reach out via [LinkedIn](https://www.linkedin.com/in/abhijit-mandape) or [Email](mailto:abhijit.mandape@gmail.com).
