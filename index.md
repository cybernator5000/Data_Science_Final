## Data Science Project: Billboard Top 100
```markdown
First thing first is Imports. there are a lot, but I use most if not all of them throughout the code so it's justifiale.
```
{
 "cells": [
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "d8b9933e",
   "metadata": {},
   "outputs": [],
   "source": [
    "from numpy import random\n",
    "import numpy \n",
    "import re\n",
    "import os\n",
    "import requests\n",
    "from bs4 import BeautifulSoup\n",
    "from bs4.element import Comment\n",
    "import urllib.request\n",
    "import shutil\n",
    "from time import sleep\n",
    "import pandas as pd\n",
    "from matplotlib.ticker import FormatStrFormatter\n",
    "from matplotlib import pyplot as plt\n",
    "from matplotlib.pyplot import figure\n",
    "from random import randint, randrange\n",
    "from sklearn import tree\n",
    "from sklearn.ensemble import RandomForestClassifier\n",
    "from sklearn.neighbors import KNeighborsClassifier\n",
    "from sklearn import linear_model, metrics, preprocessing\n",
    "from sklearn.preprocessing import StandardScaler, MinMaxScaler\n",
    "from sklearn.linear_model import LogisticRegression, LinearRegression\n",
    "from sklearn.model_selection import train_test_split\n",
    "from sklearn.metrics import r2_score, f1_score\n",
    "\n",
    "\n"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.8.8"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}


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
