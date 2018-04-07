# Scripts in this directory


## scrape_blogs.ipynb

* Performs a number of tasks for each blog
  - Creates a directory in ../confidential for the blog
  - Spider the site using scrapy to find all in-site url references to the site's blog posts (using regex to define what a blog text (as opposed to a listing of posts or index page, etc.) looks like)
  - Gets all unique blog text urls
  - Goes to each url and extracts the text as a corpus
  - Saves corpus to a file within the blog's directory


## analyze_blogs.ipynb
  - Analyzes corpus for parts of speech
  - Analyzes corpus for topics (important for matching)
  - Saves data about blog in deidentified way (using blog id #)


## stats_blogs.ipynb

  - Compare case and control corpora using statistical tests
  - Identify outliers
  - Visualize findings