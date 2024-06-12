# Ani-Spider

Ani-Spider is a web scraping tool built using Scrapy, a powerful and flexible web crawling and web scraping framework for Python. This project is designed to scrape data from the MyAnimeList website efficiently.

## Table of Contents
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Features
- **Efficient Web Scraping**: Utilizes Scrapy's features to efficiently scrape data from websites.
- **Customizable**: Easily configurable settings for tailored scraping needs.
- **Extensible**: Can be extended with custom spiders for specific websites.

## Requirements
- Python 3.x
- Scrapy

## Installation
To install and run the project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/manoj-323/ani_spider.git
   cd ani_spider
   ```

2. **Create a virtual environment and activate it:**
   ```bash
   python -m venv env
   source env/bin/activate   # On Windows use `env\Scripts\activate`
   ```

3. **Install the required dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## Usage
To start using the web scraper:

1. **Navigate to the project directory:**
   ```bash
   cd ani_spider
   ```

2. **Run the spider:**
   ```bash
   scrapy crawl <spider_name>
   ```
   Replace `<spider_name>` with the name of the spider you wish to run.

### Available Spiders
- **web_crawler.py**: Crawls anime data such as name, stats, and other details from the MyAnimeList website.
- **img_crawler.py**: Crawls anime image links along with names from the MyAnimeList website.

### Customizing Items
Uncomment the relevant items in `items.py` according to the data being crawled. This ensures that the scraped data is properly structured and stored.

## Project Structure
- `ani_spider/`: Contains the main Scrapy project.
  - `spiders/`: Directory to store the spiders.
    - `web_crawler.py`: Spider for crawling anime data.
    - `img_crawler.py`: Spider for crawling anime images.
  - `items.py`: Defines the data structures for the scraped items.
  - `pipelines.py`: Contains logic for data cleaning.
  - `middlewares.py`: Contains custom middleware for convenient scraping.
  - `settings.py`: Configuration settings for the Scrapy project.
- `scrapy.cfg`: The project configuration file.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request for any features, improvements, or bug fixes.

### Steps to Contribute
1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- [Scrapy](https://scrapy.org) - An open-source and collaborative web crawling framework for Python.
