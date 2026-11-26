
# Spotify Music Trends Dashboard

An interactive music analytics dashboard built with Python and Streamlit to explore Spotify track data, music popularity, genre patterns, artist rankings, and audio characteristics.

## Project Overview

The Spotify Music Trends Dashboard explores patterns in music data through interactive visualizations and analytical indicators. It examines how tracks perform in terms of popularity and how different audio characteristics, such as danceability, energy, tempo, and valence, are distributed across the dataset.

The project combines data preprocessing, exploratory data analysis, and interactive visualization to make music-related data easier to explore and interpret.

## Project Objectives

- Analyze track popularity and identify patterns across music genres.
- Compare genres based on average track popularity.
- Identify artists and tracks with the highest popularity scores.
- Explore relationships between audio features such as danceability, energy, tempo, and valence.
- Examine the distribution of popularity and audio characteristics.
- Present music data through an interactive dashboard.

## Dataset

The project uses `train.csv`, a track-level dataset containing information about music tracks, artists, albums, genres, popularity, and audio features.

### Key Dataset Attributes

- Track Name
- Artist
- Album
- Genre
- Popularity
- Danceability
- Energy
- Tempo
- Valence
- Duration
- Explicit Content

The dashboard also generates additional analytical categories, including:

- **Popularity Category:** Low, Medium, and High Popularity.
- **Mood Category:** Low Valence, Balanced Valence, and High Valence.
- **Explicit Content Label:** Explicit and Clean.
- **Track Duration:** Converted from milliseconds into minutes.

## Methodology

The project follows these analytical procedures:

1. **Data Loading** – Imported the Spotify track dataset using Pandas.
2. **Data Cleaning** – Standardized column names, removed unnecessary index columns, handled missing display fields, and removed exact duplicate records.
3. **Data Transformation** – Converted track duration into minutes and generated popularity, mood, and explicit-content categories.
4. **Exploratory Data Analysis** – Examined track popularity, genre distribution, artist performance, and audio characteristics.
5. **Data Visualization** – Created interactive charts to explore patterns and relationships among the selected variables.
6. **Dashboard Development** – Integrated the visualizations and interactive filters into a Streamlit application.

## Interactive Dashboard

The project features a Streamlit dashboard titled **Spotify Music Trends Dashboard**, designed with a dark interface and Spotify-inspired green accents.

### Dashboard Features

**1. Key Performance Indicators**

Displays summary metrics such as:

- Total Tracks
- Average Popularity
- Average Danceability
- Average Energy
- Average Tempo

**2. Genre Analysis**

Compares music genres based on average popularity and explores genre-level patterns.

**3. Popularity Analysis**

Examines track popularity scores and their distribution across low, medium, and high popularity categories.

**4. Audio Feature Analysis**

Explores relationships between selected audio characteristics, including:

- Danceability and Popularity
- Energy and Valence
- Other numerical audio features

**5. Artist and Track Rankings**

Identifies top-performing artists and tracks based on popularity.

**6. Correlation Analysis**

Uses a correlation heatmap to examine relationships among numerical music attributes.

**7. Interactive Filters**

Allows users to explore the dataset using filters for:

- Music Genre
- Popularity
- Energy
- Danceability
- Explicit Content
- Track and Artist Search

## Dashboard Preview

Screenshots of the dashboard are available in the `screenshots` folder.

<!-- Update the image filenames below to match the actual uploaded screenshots. -->

![Dashboard Overview](screenshots/dashboard-overview.png)

![Genre Analysis](screenshots/genre-analysis.png)

![Audio Feature Analysis](screenshots/audio-features.png)

![Correlation Heatmap](screenshots/correlation-heatmap.png)

## Technologies Used

- **Python** – Main programming language
- **Pandas** – Data cleaning, manipulation, and analysis
- **NumPy** – Numerical operations and data transformation
- **Plotly Express** – Interactive data visualization
- **Plotly Graph Objects** – Customized charts and visualizations
- **Streamlit** – Interactive dashboard development

## Repository Contents

| File or Folder | Description |
|---|---|
| `spotify_dashboard_app.py` | Main Streamlit dashboard application |
| `train.csv` | Track-level dataset used by the dashboard |
| `requirements.txt` | Python project dependencies |
| `screenshots/` | Dashboard screenshots |
| `README.md` | Project documentation |
| `LICENSE` | Project license |

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/RalphIlarde/spotify-music-trends-dashboard.git
```

### 2. Navigate to the Project Directory

```bash
cd spotify-music-trends-dashboard
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Dashboard

```bash
python -m streamlit run spotify_dashboard_app.py
```

The dashboard will open in your default browser.

## Project Insights

The dashboard provides an interactive way to examine music popularity, genre patterns, artist rankings, and audio characteristics.

It allows users to explore how different audio features are distributed across tracks and investigate their relationships with popularity. These visualizations support descriptive analysis and do not establish causal relationships.

## Author and Contributors

**Ralph Victor Ilarde**  
BS Information Systems – Business Analytics  
West Visayas State University

**Team Members:**
- Ralph Victor L. Ilarde
- Adrielle Arcos
- Charmaine Cachila

GitHub: [RalphIlarde](https://github.com/RalphIlarde)

## License

This project is distributed under the GNU General Public License v2.0 (GPL-2.0). See the `LICENSE` file for details.
