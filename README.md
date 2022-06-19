# Replit-Node
A file to update Node on Replit


Installation

1. Copy this scripts inside the ``scripts`` section on package.json
```
"node-update": "npm i --save-dev node@17 && npm config set prefix=$(pwd)/node_modules/node && export PATH=$(pwd)/node_modules/node/bin:$PATH",
"node-clean": "rm -rf node_modules && rm package-lock.json && npm cache clear --force && npm cache clean --force && npm i",
"replit-node": "npm run node-update && npm run node-clean"
```
2. On shell execute ``npm run replit-node``
3. Success now you have Node v17 on ur Replit, you only need to do this one time

- Cooming soon npm updater, stay tuned
