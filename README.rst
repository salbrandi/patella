A Webservice for Scraping Files and Plotting Data Against Presidential Party Variation
=====================================================================================

``patella`` uses Flask to host an interactive html/css/js frontend through which users can navigate to
data and plot it.




Flask Url Paths
---------------

``patella`` uses the  http ``GET`` and ``POST`` commands to send data between
one page and another. The homepage is ``/`` and ``/index``, from which you can
navigate to the rest of the front end.



Install and Run Directions
--------------------------

``patella`` is uploaded to the pip package repository.

To install, simply run ``pip install patella``. A ``requirements.txt``
file that comes with the package specifies its dependencies. Install these with
``pip install -r requirements.txt``. It is recommended you run this in a virtual
so as not to interfere with previous installations.

To start the flask server, run ``patella startup <URL>``, where URL is the path
to be prepended to the page url. Next, use a browser to browse to
``127.0.0.1:4444`` and begin using the webservice.


Files
-----

Log files
Data files