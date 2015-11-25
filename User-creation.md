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

Creating an account is also possible with oAuth2.

Follow the classic oAuth2 flow.

/!\ Only Facebook and Google+ are available for account creation on oAuth 