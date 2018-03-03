# Scripts in this directory


## scrape_blogs.ipynb

* Performs a number of tasks for each blog
  - Spider the site using scrapy to find all in-site url references to the site's blog posts (using regex to define what a blog text (as opposed to a listing of posts or index page, etc.) looks like)
  - Gets all unique blog text urls
  - Goes to each url and extracts the text, adding it to a corpus of the blog texts for that blog
  - Analyzes corpus for parts of speech
  - Analyzes corpus for topics (important for matching)
  - Saves data about blog in deidentified way (using blog id #)


## analyze_blogs.ipynb

  - Compare case and control corpora using statistical tests
  - Identify outliers
  - Visualize findings