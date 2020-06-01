# Livepeer VSP RTMP

> Example on how to create a live streaming video service platform using Livepeer's API

## Usage

Install [NVM](https://github.com/nvm-sh/nvm)

Use v12.17.0

```
nvm install v12.17.0
nvm use v12.17.0
```

Install Dependencies
```
cd livepeer-vsp-rtmp
```

Start Service
```
yarn dev
```

Running the production build on localhost. This will create a production build, then Node will serve the app on http://localhost:5000

```
NODE_ENV=production yarn dev:server
```

## How this works

The client talks to the backend express service through a proxy.  We have a _proxy_ entry in `client/package.json`
```
"proxy": "http://localhost:5000/"
```

## Livepeer
For more information about Livepeer, visit [www.livepeer.com](https://livepeer.com)