# Scrape YouTube comments

```scraper_yt``` is a package which allows the user to scrape comments off of YouTube videos with ease.

- Free software: MIT license

## Installation

```pip install scraper_yt``` 

## Tutorial

```
import scraper_yt CommentsScraper

# The path where the Chrome driver is stored on your local machine
PATH = r"C:\Program Files (x86)\chromedriver.exe"

# The link of the YouTube video whose comments you want to scrape
vid = "https://www.youtube.com/watch?v=HFtJbRKuwtI&list=PLLssT5z_DsK-h9vYZkQkYNWcItqhlRJLN&index=28"

# The number of comments you want to scrape
num = 15

# Create an instance of CommentsScraper and pass the PATH variable into it 
# Call the commentsTpDataFrame() method and pass in the vid and num variables 
df = CommentsScraper(PATH).commentsToDataFrame(vid, num)

print(df)
```

## Changelog

#### 0.1.0 (2020-11-18)

- First release on PyPI.
