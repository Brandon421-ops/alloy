# Deployment

Table of contents

- Quick & easy deployment
- Deployment configuration explaination
- how to use email OTP Verification mode
- Advanced Deployment
- Filesystem

## Quick & Easy Deployment Options

[![Deploy to Heroku](https://raw.githubusercontent.com/BinBashBanana/deploy-buttons/master/buttons/remade/heroku.svg)](https://heroku.com/deploy/?template=https://github.com/NebulaServices/alloy)
<br>
[![Run on Replit](https://raw.githubusercontent.com/BinBashBanana/deploy-buttons/master/buttons/remade/replit.svg)](https://replit.com/github/Brandon421-ops/alloy)
<br>
[![Deploy to IBM Cloud](https://raw.githubusercontent.com/BinBashBanana/deploy-buttons/master/buttons/remade/ibmcloud.svg)](https://cloud.ibm.com/devops/setup/deploy?repository=https://github.com/Brandon421-ops/alloy)
<br>
[![Deploy to Amplify Console](https://raw.githubusercontent.com/BinBashBanana/deploy-buttons/master/buttons/remade/amplifyconsole.svg)](https://console.aws.amazon.com/amplify/home#/deploy?repo=https://github.com/Brandon421-ops/alloy)
<br>
[![Run on Google Cloud](https://raw.githubusercontent.com/BinBashBanana/deploy-buttons/master/buttons/remade/googlecloud.svg)](https://deploy.cloud.run/?git_repo=https://github.com/Brandon421-ops/alloy)
<br>
[![Deploy on Railway](https://binbashbanana.github.io/deploy-buttons/buttons/remade/railway.svg)](https://railway.app/new/template/pBzeiN)
<br>
[![Deploy To Koyeb](https://binbashbanana.github.io/deploy-buttons/buttons/remade/koyeb.svg)](https://app.koyeb.com/deploy?type=git&repository=github.com/Brandon421-ops/alloy&branch=main&name=alloy)
<br>
[![Deploy to Render](https://raw.githubusercontent.com/BinBashBanana/deploy-buttons/main/buttons/remade/render.svg)](https://render.com/deploy?repo=https://github.com/Brandon421-ops/alloy)
<br>
[![Remix on Glitch](https://binbashbanana.github.io/deploy-buttons/buttons/remade/glitch.svg)](https://glitch.com/edit/#!/import/github/Brandon421-ops/alloy)

## Running locally

```sh
git clone https://github.com/titaniumnetwork-dev/alloyproxy.git
cd alloyproxy
node server.js
```


## Options in config.json
```json
{
    "port": "8080",
    "ssl": false,
    "prefix": "/web/",
    "localAddresses": [],
    "blockedHostnames": []
}
```

`"port": "8080"` = Sets HTTP server port of web proxy.

`"ssl": "false"` = Sets HTTP server SSL.

`"prefix": "/web/"` = Sets the overall prefix of the web proxy.

`"localAddresses": [ "0.0.0.0" ]` = Allows you to choose which IP to make the request from. If there are multiple IP's then the IP chosen will be randomized.

`"blockedHostnames": [ "example.org", "example.com" ]` = If the hostname of the proxy URL matches any of the URL hostnames listed in the array, the request to the server will be cancelled.
