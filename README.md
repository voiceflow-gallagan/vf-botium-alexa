# vf-botium-alexa

## Install Botium and Amazon Alexa Skills API Connector

> Based on the documentation here: https://github.com/codeforequity-at/botium-connector-alexa-smapi/tree/8513ea4c89a42a623a79642e8ced591af7574598

```
> npm install -g botium-bindings
> npm install -g botium-connector-alexa-smapi
> npm install
```

## Connecting Amazon Alexa Skills API to Botium

This connector includes a CLI wizard to initialize the botium.json file holding your connection credentials.

```
> npx botium-connector-alexa-smapi-cli init
```

This wizard will guide you through the Botium Connector setup. Please follow the instructions.
It involves Copy&Paste from a web browser to this terminal window.


## Adapt botium.json

Be sure that the botium.json file created by the wizard has the **ALEXA_SMAPI_API** set to **simulation**.

```
"ALEXA_SMAPI_API": "simulation",
```

## Create your test convo

In the convo directory, you can add multiple scripts to test your Alexa skill

More info on the official documentation here: https://botium-docs.readthedocs.io/en/latest/

## Run your test

```
> npm test
```

