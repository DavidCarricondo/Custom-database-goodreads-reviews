# Custom-database-goodreads-reviews

<img src='Goodreads.jpeg' width=600 height=200>

Custom reviews-database created from scrapping goodreads.com.


I used **Selenium** to automate the scrapping of the latest 60 reviews posted in the website of more than 1000 titles. Take a look at [the code](https://github.com/DavidCarricondo/Custom-database-goodreads-reviews/blob/master/src/scrap_dataset.py)!!

## The result
The data comes in two flavors. The raw results is a [**json** file](https://github.com/DavidCarricondo/Custom-database-goodreads-reviews/blob/master/DATA/goodread_reviews_dataset.json) with the following format:

<pre><code>
{"0": {"review": "...", 
        "grade": "it was amazing"}, 
"1": {"review": "I can see Never Let Me Go being great for book clubs ...", 
    "grade":"it was ok"},
...
}
</code></pre>

Note: Grades reflect the website grading. This is:
+   'did not like it': 1 star
+   'it was ok': 2 stars
+   'liked it': 3 stars
+   'really liked it': 4 stars
+   'it was amazing': 5 stars
