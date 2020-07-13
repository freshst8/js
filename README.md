<h1>Content Grabber</h1>
<p>This pulls in a requested document from remote host through using PHP's file_get_contents()</p>
<p>JQuery is then available to traverse the information as needed and grab whatever you need</p>
<p>After much fighting with CORS errors and trying to set everything in Apache's http.conf, to no avail, it was
easier to just have PHP make the request and then have Jquery grab that content with $.get(). In grab.html I didn't go much further than to take the data retrieved from PHP ("get.php" in this case) and have it inserted into a DIV.</p>
