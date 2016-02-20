# Nostradamus

The EdenBeat API has a prediction module.
```
GET `nostradamus?query=test`
```

will return all artists matching with test.

This route can be called when the user types in a search field to show suggestions.

Each artist has an ID.

Call the route again with the parameter id=ARTIST_ID to get news, biography, images related to the artist, similar artists and top songs
```
GET `nostradamus?id=ARRH63Y1187FB47783`
```
