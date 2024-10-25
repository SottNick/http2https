This is a simple PHP script to create a gateway to access HTTPS (SSL) web pages and files via HTTP requests.

This script may be needed, for example, for Arduino-based devices (ESP6266) when there is no option to support SSL certificates. 

After placing the index.php file on the web server in the folder intended for the website, you will be able to open links of the format
http://MY_SITE.com/?https://api.weather.yandex.ru/v2/...
thereby retrieving the content of the link shown after the question mark.

If you want to place the gateway script not on a separate domain, but on the domain of a running website, use the name http2https.php.
In this case the link will be
http://MY_SITE.com/http2https.php?https://api.weather.yandex.ru/v2/...

Make sure that your web server does not automatically redirect http:// links to https://, or set an exception for the http2https.php file.
