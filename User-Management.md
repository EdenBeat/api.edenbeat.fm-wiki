## User Management

### User Creation

User can be created two ways:

By making a ```POST /user``` request

By initiating an oAuth2 flow with one of the services. For this second method, see "Account Linking".

```POST /user```
required body params:
```
{
  "password": "userPassword",
  "email": "userEmail"
}
```

/!\ Note that the "username" can also be specified. If not, it will be generated using the mail address.

## Retrieving a user

```GET /user/self```

## Modifying a user

```PUT /user/self```
Accepted parameters:
```
{
  "password": "userPassword",
  "email": "userEmail"
  "username"
}
```

## Account linking

First, read this, seriously: https://en.wikipedia.org/wiki/OAuth

The various fronts (website/apps) first need to require the oAuth link url from the API.