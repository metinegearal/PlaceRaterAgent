# 📍 PlaceRaterBot - Review-Based Place Rating Agent

This notebook uses generative AI to analyze and rate places (like restaurants, cafes, or bars) based on user reviews. It combines Google Maps metadata with LLM-powered sentiment analysis and scoring to help users quickly evaluate and compare multiple locations.

## 🔍 Features

- Accepts review text from up to 20 places (5 recommended)
- Uses a language model (e.g., GPT or Gemini) to extract sentiment trends
- Outputs comparative ratings with explanations
- Optional visualization of rating breakdowns
- Can be connected to Google Maps API for coordinates, name, or nearby search
  
##📊 Example Output
name and location = Beytna, [40.45686560000001, -3.6481194]
rate=  
Middle Eastern Cuisine 4,
Hummus 4.5,
Tabbouleh 4, …
Summary = It's like rate, but with additional information about pointing 
Middle Eastern Cuisine: Good (authentic Middle Eastern cuisine), 
Hummus: Excellent (creamy and flavorful),
Tabbouleh: Good (fresh and zesty),\ …

##🚀 How to Run
1. Clone the repository:

   ```bash
   git clone https://github.com/metinegearal/PlaceRaterBot.git
   cd PlaceRaterBot
   ```
2. Open the notebook in Jupyter or VSCode
3. Take a Google Maps and Gemini API, put it in the fifth cell directly, or if you are using kaggle notebooks, you can put it in the secrets page
   
Google Maps Platform API
https://developers.google.com/maps/documentation/places/web-service
https://developers.google.com/maps/documentation/geocoding
Gemini API
https://console.cloud.google.com/apis/library/generativelanguage.googleapis.com

```python
   # getting keys
   from kaggle_secrets import UserSecretsClient
   GOOGLE_API_KEY = UserSecretsClient().get_secret('GOOGLE_API_KEY') # gemini's key
   MAPS_API_KEY = UserSecretsClient().get_secret('MAPS_API_KEY') # Google Maps Platform API, dont forget to enable geocoding and    
```

4. You can write your need in the "Try by yourself" title's first cell 
5. Try something:

Rate 10 restaurants near Tokyo center one by one, don't forget fast food ones, and add specific dishes to the summary
what should ı eat in Tokyo(give with place name) according to rating
I am near Arturo Soria Plaza in Madrid. ı am really hungry, can you give me some place options in a 15-minute walking range

6. You can see the results with the map in the GUI part

## 📓 Some Warnings
This project is not totally finished, and there can be problems:
1. Because of the details in the reviews, it can stop early, either you should say continue or restart the current cell(There is a control mechanism which sometimes doesn't work)
2. Lack of reviews or overgeneralization can be problematic.
3. Some unorganized code.
If you find another mistake or a solution, let me know.

##🌐 Outer links
Blog: https://medium.com/@metinegearal/place-rater-agent-6f15ccadf62a
Kaggle notebook: https://www.kaggle.com/code/metinegearal/place-rater-bot
