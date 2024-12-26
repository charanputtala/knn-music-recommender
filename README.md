# KNN Music Recommender


A simple yet effective music recommendation system built using the **K-Nearest Neighbors (KNN)** algorithm. This project normalizes song features such as danceability, energy, and tempo to recommend similar tracks based on a user's input.

---

## Features

- Recommends songs based on similarity in musical attributes.
- Normalizes features for better comparison and accuracy.
- Lightweight and easy to understand for beginners.

---

## Table of Contents

1. [Demo](#demo)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Dataset](#dataset)
5. [Contributing](#contributing)
6. [License](#license)

---

## Demo

Input a song ID, and the system suggests the top 5 most similar songs:

| **Input Song**  | **Recommended Songs**        |
|------------------|-----------------------------|
| Song: "S0001"    | Song 1: "S0003"             |
|                 | Song 2: "S0005"             |
|                 | Song 3: "S0010"             |
|                 | Song 4: "S0008"             |
|                 | Song 5: "S0002"             |

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/knn-music-recommender.git
   ```
2. Navigate to the project directory:
   ```bash
   cd knn-music-recommender
   ```
3. Install required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

1. Launch the script in your Python environment (e.g., Google Colab or Jupyter Notebook).

2. Load the dataset using the following code:
   ```python
   import pandas as pd

   music_data = pd.read_csv("synthetic_music_dataset.csv")
   ```

3. Run the recommendation function:
   ```python
   recommended_songs = recommend_songs("S0001", k=5)
   print(recommended_songs)
   ```

4. Output:
   ```
   Song_ID  Title     Artist     Genre
   S0003    Song 3    Artist 13  Pop
   S0005    Song 5    Artist 5   Rock
   ...
   ```

---

## Dataset

The dataset is a synthetic music dataset containing the following columns:

- **Song_ID**: Unique identifier for each song.
- **Title**: Name of the song.
- **Artist**: Artist name.
- **Danceability**: A measure of how suitable a track is for dancing.
- **Energy**: Intensity and activity level of the track.
- **Tempo**: The speed of the track in beats per minute.
- **Genre**: The genre of the song.

---

## Contributing

Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-branch-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add some feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-branch-name
   ```
5. Open a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

