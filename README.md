# 📍 PlaceRaterBot - Review-Based Place Rating Agent

This notebook uses generative AI to analyze and rate places (like restaurants, cafes, or bars) based on user reviews. It combines Google Maps metadata with LLM-powered sentiment analysis and scoring to help users quickly evaluate and compare multiple locations.

## 🔍 Features

- Accepts review text from 1 to 5 places
- Uses a language model (e.g., GPT or Gemini) to extract sentiment trends
- Outputs comparative ratings with explanations
- Optional visualization of rating breakdowns
- Can be connected to Google Maps API for coordinates, name, or nearby search

## 📓 File Structure

1. Clone the repository:

   ```bash
   git clone https://github.com/metinegearal/PlaceRaterBot.git
   cd PlaceRaterBot
   ```
  Open the notebook in Jupyter or VSCode:

  ```bash
  jupyter notebook place_rater_bot.ipynb
  ```
  Paste your reviews into the input cell.
  
Run the notebook to see place-wise ratings and summaries.
