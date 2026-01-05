# Chess Opening Recommendation System

## Overview
The Chess Opening Recommendation System  classifies chess openings into play-style categories, using early-game moves as the primary input. The system predicts whether a player's play-style is **Classical**, **Positional**, **Tactical**, **Hypermodern**, **Dynamic**, or **Sharp**.

The system uses:
- **Opening move data** (ECO codes and statistics)
- **Real-world game data** (moves, outcomes, player ratings)
- **Live Chess.com API** data for recent game analysis
- **Feature engineering** applied to the first 8 ply of a game
- **Random Forest classifier** to predict play-styles

## Key Features
- Predicts chess play-styles based on opening moves and player ratings.
- Uses real-time game data from Chess.com for inference.
- Trained with a **Random Forest classifier** to provide robust predictions.
- **Test Accuracy**: 94%
- **Balanced Accuracy**: 95%
- **F1 Score**: 94% (Weighted)

## Model Overview
The system utilizes a **Random Forest classifier**, trained on the following features:
- Player colour (White/Black)
- Player rating
- Encoded move sequences (move1w to move4b)

## How It Works
1. **Data Processing**: The system processes ECO codes, player ratings, and game moves, applying feature engineering to generate a structured dataset.
2. **Model Training**: A Random Forest model is trained on labeled data (from ECO codes and opening names) to predict play-style.
3. **Live Inference**: The model predicts play-styles for real-time Chess.com game data, fetching recent games via the API.

---

**Contact:**  
Tom Handley | [LinkedIn](www.linkedin.com/in/tom-handley-a8a0791a6) | [Email](mailto:tomhandley100@gmail.com)
