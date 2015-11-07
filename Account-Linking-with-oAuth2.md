## Account linking

First, read this, seriously: https://en.wikipedia.org/wiki/OAuth

The various fronts (website/apps) first need to require the oAuth link url from the API.

```GET /services/:slug/link```

Where :slug is the name of the service, Facebook for example

The API will redirect your request using a 302 to the actual service link page.

So, the easy way to implement this is:
  - Open a new browser window and set the url to ```{API_URL}/services/:slug/link```
  - The API will automatically redirect this window to the oAuth flow