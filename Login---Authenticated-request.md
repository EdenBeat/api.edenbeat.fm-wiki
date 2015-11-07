## Login

To login you must use the following route:

```POST /login```

Specify the email adress and the password in the request body.

In the response header, you will find a Session-Id field.
Carry this field value on every request you make to make authenticated requests.

## Logout

Just do a ```GET /logout``` (don't forget to specify your Session-Id in the headers)