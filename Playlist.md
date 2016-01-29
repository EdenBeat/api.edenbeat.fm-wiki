## Accessing a playlist

/!\ For now, only the playlist ID is needed since user ID are hard coded /!\

We currently support the following services:
* Soundcloud
* Deezer
- Spotify is implemented but not yet supported since the oAuth is broken.

A search can be done by sending a ```GET``` request on the search endpoint ```/importplaylist/name_service````

Example:
```GET /importplaylist/deezer?id=943784415````