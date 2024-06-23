# weather-app-python
using django and open weather api 
# Weather Project

A Django-based weather application that fetches and displays weather information for a specified city using the OpenWeatherMap API.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Features

- Fetches current weather data for a specified city.
- Displays temperature, weather description, and an icon representing the weather.
- Dynamically fetches a city image from Google Custom Search API.
- Responsive design.

## Prerequisites

- Python 3.x
- Django 3.1.6 or later
- OpenWeatherMap API key
- Google Custom Search API key and Search Engine ID

## Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/yourusername/weatherproject.git
    cd weatherproject
    ```

2. Create a virtual environment and activate it:

    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:

    ```sh
    pip install -r requirements.txt
    ```

4. Set up environment variables:

    Create a `.env` file in the root of the project and add your API keys:

    ```plaintext
    SECRET_KEY='your-django-secret-key'
    DEBUG=True
    OPENWEATHERMAP_API_KEY='your-openweathermap-api-key'
    GOOGLE_API_KEY='your-google-api-key'
    GOOGLE_SEARCH_ENGINE_ID='your-google-search-engine-id'
    ```

5. Run the database migrations:

    ```sh
    python manage.py migrate
    ```

6. Start the development server:

    ```sh
    python manage.py runserver
    ```

## Usage

1. Open your web browser and go to `http://127.0.0.1:8000/`.
2. Enter a city name and click the submit button to fetch and display the weather information.

## Configuration

- **OpenWeatherMap API**: Sign up at [OpenWeatherMap](https://home.openweathermap.org/users/sign_up) to get your API key.
- **Google Custom Search API**: Set up a custom search engine at [Google Custom Search](https://cse.google.com/cse/) and obtain your API key and Search Engine ID.

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
