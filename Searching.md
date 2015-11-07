## Supported services

/!\ Search is currently a non restricted endpoint /!\

We currently support the following services:
* Mixcloud
* Deezer
* Spotify
* SoundCloud

A search can be done by sending a ```GET``` request on the search endpoint ```/search````

Example:
```GET /search?query=test````

## Accepted parameters

* services (specify a service to restrict the search on)
* type (specify a type to search on)

The following types are supported:

* artists
* tracks

Example:

```GET /search?query=test&services=soundcloud&type=tracks```