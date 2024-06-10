# spotify-data-script


This Jupyter notebook is designed to interact with the Spotify API to fetch and analyze data on top artists. It demonstrates how to authenticate with the API, retrieve data, and process it for analysis.

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Notebook Structure](#notebook-structure)
- [Important Functions](#important-functions)
- [Notes](#notes)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This notebook aims to provide a step-by-step guide to fetch data from the Spotify API. It covers the following aspects:
- Authentication with the Spotify API.
- Fetching data about top artists.
- Processing and visualizing the data.

## Requirements

To run this notebook, you will need:
- Python 3.6 or higher
- Jupyter Notebook
- Spotify Developer Account with a registered application to get the `client_id` and `client_secret`.

## Installation

1. Clone the repository or download the notebook.

   ```bash
   git clone https://github.com/yourusername/spotify-data-fetcher.git
   cd spotify-data-fetcher
   ```

2. Install the required Python packages using pip:

   ```bash
   pip install -r requirements.txt
   ```

   The `requirements.txt` should contain:

   ```plaintext
   requests
   pandas
   matplotlib
   python-dotenv
   ```

3. Create a `.env` file in the same directory as your notebook and add your Spotify credentials:

   ```plaintext
   SPOTIFY_CLIENT_ID=your_client_id
   SPOTIFY_CLIENT_SECRET=your_client_secret
   ```

## Usage

1. Open the Jupyter notebook.

   ```bash
   jupyter notebook spotify.ipynb
   ```

2. Run the cells in order. The notebook will:
   - Load the required libraries.
   - Authenticate with the Spotify API using your credentials.
   - Fetch data about the top 10 artists from a popular Spotify playlist.
   - Display the data in a readable format and plot visualizations.

## Notebook Structure

The notebook is divided into the following sections:

1. **Setup and Imports**: Import necessary libraries and load environment variables.
2. **Authentication**: Fetch Spotify API credentials and obtain an access token.
3. **Data Retrieval**: Define functions to get data from the Spotify API.
4. **Data Processing**: Process the retrieved data to extract relevant information.
5. **Visualization**: Create visualizations to analyze the data.

## Important Functions

- `get_token()`: Authenticates with the Spotify API and returns an access token.
- `get_top_10_artists(access_token)`: Retrieves data about the top 10 artists from a specific Spotify playlist.

## Notes

- Ensure that your Spotify API credentials are kept secure and not shared publicly.
- This notebook fetches data using the Spotify API, so you must comply with their terms of use.
- The API token has a limited validity period, and you may need to re-authenticate to get a new token.

## Contributing

Contributions are welcome! If you find any bugs or have suggestions for improvements, please create an issue or submit a pull request on the GitHub repository.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

