# api.edenbeat.fm

This document explains how to interact with the EdenBeat API

## About

The EdenBeat API is a REST API that serves requests for the various EdenBeat frontends (Mobile apps and website)

This API has a token based authentification built on top of a REDIS database.

User profiles and data are stored in MongoDB.

### Endpoints

This API exposes various endpoints following the REST convention, you can find the API documentation on DOC.md /*Needs to be created*/

### Contributing

To start the EdenBeat api you will need:

	* A local mongo server running
  ```
  mkdir .db
  sudo mongod --dbpath .db/
  ```

	* A local redis server running
  ``` redis-server ```

Then, just type ```node bin/server``` and start doing requests on http://localhost:8000 or whatever shitty port you set in your config

/!\ Your cannot be merged if: /!\

  - You have callbacks hells
  - You don't write tests
  - Any test fail on circleci

A POSTMAN library can be found in the documentation folder.

### Tests

Test are run using mocha, just type ```npm test```
Some tests can fail because of timeouts. The distant API's can't take a little bit longer than usual to respond.
