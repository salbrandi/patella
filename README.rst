A Webservice for Scraping Files and Plotting Data Against Presidential Party Variation
======================================================================================

``patella`` uses Flask to host an interactive html/css/js frontend through which users can navigate to
data and plot it.




Flask Url Paths
---------------

``patella`` uses the  http ``GET`` and ``POST`` commands to send data between
one page and another. The homepage paths are ``/`` and ``/index`` from which you can
navigate to the rest of the front end.



Install and Run Directions
--------------------------

``patella`` is uploaded to the pip package repository.

To install, simply run ``pip install patella``\ . A ``requirements.txt`` file that comes with the
package specifies its dependencies. Install these with ``pip install -r requirements.txt``\ . It is
recommended you run this in a virtual environment so as not to interfere with previous installations.

To start the Flask server, run ``patella startup <URL>``\ , where URL is the path
to be prepended to the page url. Next, use a browser to browse to ``127.0.0.1:4444``\ .
To access the service from other computers on the same network, use the public ip of the host
computer on port 4444. From these two addresses the webservice can be accessed as long as the server is running.


Files
-----

Log Files
+++++++++
A log file will be generated in the path that you run the webservice from named
``webservice.log``. this file includes server reloads, error reporting, logs get
and post requests and debugger pins. ``POST`` and ``GET`` logs are timestamped, but others are not


Data Files
++++++++++
Data files from the webservice will be downloaded to a ``data/`` directory created at runtime in the directory the
server is started from. In that directory, all files downloaded from the webservice will be browseable.