set up server
```
git clone https://github.com/Throbac-Labs/secure-server-setup.git
```
clone repo
```
git clone https://github.com/thodges-gh/CL-EA-NodeJS-Template.git ExternalAdapterProject
cd ExternalAdapterProject
```
install dependencies
```
yarn
yarn test
```
set up dotenv for api key verification
```
yarn add dotenv
```
add api key
```
# add below 1st line of code in index.js
require('dotenv').config() 
var apiKey = process.env.API_KEY

# create .env
nano .env
API_KEY=Your-Api-Key
```
edit index.js
```
# edit cutomParams -- setting params necessary to build url
# edit createRequest -- building url
# edit params -- setting params that are used for the request
```

test with curl
```
curl -X POST -H "content-type:application/json" "http://localhost:8080/" --data '{ "id": 1, "data": {"playerId":Your-Player-ID } }'
```

https://www.youtube.com/watch?v=DJ-EYU-7f0U&t=663s
