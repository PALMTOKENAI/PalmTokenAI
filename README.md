### PALM AI Token Launcher

### What do you need?

-Node.js

-Google Cloud Console AccessToken

-DallE Key (OpenAI)

-Hardhat development environment


### Setup

Clone the repository.

run ```npm install```

Copy ```.env.example``` and rename it to ```.env```

Modify PALM_API_KEY,DALLEE_API_KEY, Private key and Rpc url

How to get Google Cloud access token

Open https://console.cloud.google.com/ , Log In

Create a billing account, add a payment method (no charges), create a project, remember it's name

Search for VERTEX AI, and press Enable API

Open https://developers.google.com/oauthplayground/

Open deploypalm.ts. find in file "appname" and "us-central1". Replace it with your own app name and region

->Step 1- Search Vertex AI API V1, click, and tick first option, press Authorize APIs

->Step 2- Log in with the same account as cloud console, Copy Access Token (Press refresh access token if its empty)

Paste Access token to .env -> PALM_API_KEY

### Running locally
```npx hardhat run scripts/deploygpt4.ts```
### Deploy to blockchain
```npx hardhat run scripts/deploygpt4.ts --network GOERLI```
