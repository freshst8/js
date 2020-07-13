<h1>grab.html, get.php</h1>
<p>This pulls in a requested document from remote host through using PHP's file_get_contents()</p>
<p>JQuery is then available to traverse the information as needed and grab whatever you need</p>
<p>After much fighting with CORS errors and trying to set everything in Apache's http.conf, to no avail, it was
easier to just have PHP make the request and then have Jquery grab that content with $.get(). In grab.html I didn't go much further than to take the data retrieved from PHP ("get.php" in this case) and have it inserted into a DIV.</p>

In fact, I noticed afterwards that Jquery's <a href="https://api.jquery.com/jQuery.get/">.get() doc</a> even pulls from PHP in it's example. Maybe they know of the troubles one may encounter trying to get CORS "Allow Origin" to work. Javascript console will direct you to <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS/Errors/CORSMissingAllowOrigin">this</a> but it's a headache unless your one of the lucky ones or are an apache guru.
