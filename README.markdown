# Placemaker CLI

This is a command-line interface to Yahoo!'s [Placemaker
API](http://developer.yahoo.com/geo/placemaker/). Placemaker is a geoparsing
web service, which means that it extracts locations from bodies of text.

## Usage

To use it, point it at a URL that you'd like locations extracted from:

    $ ./placemaker --appid=<appid> <url>

Or feed it something content directly:

    $ cat document.txt | ./placemaker --appid=<appid> --documentType=text/plain -

Optional arguments are (default):

    --documentType=mime/type        (text/html)
    --inputLanguage=lang-code       (en-US)
    --autodisambiguate=true|false   (false)
    --outputType={xml|rss}          (xml)

To register for an app id, visit https://developer.yahoo.com/wsregapp/
