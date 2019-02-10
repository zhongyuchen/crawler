# imdb-crawler

[![python version](https://img.shields.io/badge/python-3.6.7-66c2a5.svg)](https://python.org)
[![beautifulsoup4 version](https://img.shields.io/badge/beautifulsoup4-4.6.3-fc8d62.svg)](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
[![requests version](https://img.shields.io/badge/requests-2.19.1-8da0cb.svg)](http://www.python-requests.org/en/master/)
[![MIT license](https://img.shields.io/badge/license-MIT-e78ac3.svg)](https://mit-license.org)

Scrape the IMDb 50 highest rated movies and crawl the IMDb top 250 movies using python with 2 libraries, beautifulsoup4 and requests.

## Prerequisites

requirements.txt contains all the necessary packages to run the code successfully and they are easy to install with the following instruction:
```commandline
pip install -r requirements.txt
```

## Structure

```
repository-template
├── scraper
│   └── scraper.py
├── crawler
│   └── crawler.py
├── requirements.txt
├── .gitignore
├── LICENSE
└── README.md
```

## Scraper

Scrape data off the IMDb 50 highest rated movies between 2008 and 2018 using python with 2 libraries, beautifulsoup4 and requests.

### Features

* Make a copy of the target website in _movies.html_
* Scrape the data off into a csv file _movies.csv_

### Usage

```commandline
cd scraper/
python scraper.py
```

## Crawler

Scrape the IMDb top 250 movie index page for urls that lead to each movie pages.
Then crawl into each IMDb movie pages and scrape movie info.

### Features

* Make a copy of the top 250 IMDb movies index page in _index.html_
* Scrape the target urls
* Crawl into each url and scrape movie info
* Make a copy of 083 movie page in _movie-083.html_ as an example among 250 movies
* Save the top 250 IMDb movies info in a csv file _top250movies.csv_

### Usage

```commandline
cd crawler/
python crawler.py
```

## Links

* [IMDb](https://www.imdb.com)

## Author

Zhongyu Chen
