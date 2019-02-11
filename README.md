# imdb-crawler

[![python version](https://img.shields.io/badge/python-3.6.7-66c2a5.svg)](https://python.org)
[![beautifulsoup4 version](https://img.shields.io/badge/beautifulsoup4-4.6.3-fc8d62.svg)](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
[![requests version](https://img.shields.io/badge/requests-2.20.0-8da0cb.svg)](http://www.python-requests.org/en/master/)
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

Scrape data off the IMDb 50 highest rated movies between 2008 and 2018 using 2 python libraries, beautifulsoup4 and requests.

### Features

* Make a copy of [the target website](https://www.imdb.com/search/title?title_type=feature&release_date=2008-01-01,2018-01-01&num_votes=5000,&sort=user_rating,desc) in _movies.html_
* Scrape the data off into a csv file _movies.csv_

### Usage

```commandline
cd scraper/
python scraper.py
```

## Crawler

Scrape the IMDb top 250 movie index page for urls that lead to each movie pages.
Then crawl into each IMDb movie pages and scrape movie info.
These are also implemented using 2 python libraries, beautifulsoup4 and requests.

### Features

* Make a copy of [the top 250 IMDb movies index page](http://www.imdb.com/chart/top) in _index.html_
* Scrape the target urls
* Crawl into each url and scrape movie info
* Make a copy of [083 movie page](https://www.imdb.com/title/tt0986264/?pf_rd_m=A2FGELUUNOQJNL&pf_rd_p=e31d89dd-322d-4646-8962-327b42fe94b1&pf_rd_r=HC49RWRJQZT3JA01DJWC&pf_rd_s=center-1&pf_rd_t=15506&pf_rd_i=top&ref_=chttp_tt_84) in _movie-083.html_ as an example among 250 movies
* Save the top 250 IMDb movies info in a csv file _top250movies.csv_

### Usage

```commandline
cd crawler/
python crawler.py
```

## Links

* Official website [IMDb](https://www.imdb.com)
* Official datasets can be downloaded on [IMDb Datasets](https://www.imdb.com/interfaces/)

## Author

Zhongyu Chen
