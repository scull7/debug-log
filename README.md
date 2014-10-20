debug-log
=========

A simple logging mechanism built on top of debug.

Usage
-----

```javascript

var logger  = require('debug-log')('myLog')

logger.debug("Some debug message here...");
logger.info("Some info here...");
logger.warn("some warning message here...");
logger.error("some error message here...");
```

* Show all messages including debugging (useful for development)
  ```bash
  NODE_DEBUG=myLog:* node my_process.js
  ```
* Show only a specific set of messages
  ```bash
  NODE_DEBUG=myLog:error node my_process.js
  ```
