# amazon-connect-demo
amazon connect demo with callstats.js integration.

To Run
------

1. Clone the repo
2. Run "npm install"
3. Run "node index.js"

Changes in configuration (prior to RUN).
------------------------
1. Obtain the appID and appSecret from the callstats.io after creating an account (https://dashboard.callstats.io/register)  
2. Enter the appID and appSecret in app/config.js 
3. Copy paste your Amazon Connect ccpURL in app/config.js

app/config.js file contents

'use strict';

const config = {
    appId: 1234567,
    appSecret: "",
    ccpUrl: "",
    mongoUrl: "",
    mongoDatabase: "",
    mongoCollection: "",
    collectEventBusData: false
};

exports.config = config;

collectEventBusData must be true for collecting the event bus logs and storing it in the mongo.




