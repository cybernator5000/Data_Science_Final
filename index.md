## Data Science Project: Billboard Top 100
```markdown
First thing first is Imports. there are a lot, but I use most if not all of them throughout the code so it's justifiale.
```


```markdown
The first part of the project was of course, the Scraping and Crawling. By looking at our base URL (I opted for [https://www.billboard.com/charts/hot-100/2021-12-12/](url)
we can see several things:
1. The list is easily seperated into rows that are detectable via BeutifulSoup
2. The parts that aren't just given as numbers are given as unique images, such as wether a song went up or down
3. We can use the URL of the image to decipher whether or it went up, down, stayed the same or is new entirely
4. The site is very friendly to crawling, as the date field is conveniant and forgiving (if you don't use the first day of a week given, it'll just display the results
   for that week anyway)
With that information, we can start a basic scraper and crawler
```


```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```
