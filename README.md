# pushwoosh-parse-adapter
Pushwoosh push adapter for parse-server


## Installation

```
npm install --save pushwoosh-parse-adapter
```

## Usage

```
var PushwooshPushAdapter = require('pushwoosh-parse-adapter');
var pushwooshPushAdapter = new PushwooshPushAdapter({
  applicationCode: 'your-pushwoosh-app-id',
  apiAccessKey: 'your-pushwoosh-api-key'
});

var api = new ParseServer({
  push: {
    adapter: pushwooshPushAdapter
  },
  ...otherOptions
});
```