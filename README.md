[![Build Status](https://travis-ci.org/Novage/wt-tracker.svg?branch=master)](https://travis-ci.org/Novage/wt-tracker)
[![Coverage Status](https://coveralls.io/repos/github/Novage/wt-tracker/badge.svg?branch=master)](https://coveralls.io/github/Novage/wt-tracker?branch=master)
# wt-tracker
High-performance WebTorrent tracker

## Features

* handles 300k peers on single CPU thanks to [uWebSockets.js](https://github.com/uNetworking/uWebSockets.js) I/O backend
* handles HTTP and HTTPS connections simultaneously
* IPv4 and IPv6 support
* robust and well-tested: CI, unit tests, static code analyzis, 100% TypeScript
* supports tracker "scrape" extension
* statistics under /stats.json URL

## Related projects

* [p2p-media-loader](https://github.com/Novage/p2p-media-loader) - an open-source engine for P2P streaming of live and on demand video directly in a web browser HTML page
* [Novage, LLC](https://novage.com.ua/) - P2P development, support & consulting
* [WebTorrent](https://github.com/webtorrent/webtorrent) - streaming torrent client for the web https://webtorrent.io
* [uWebSockets.js](https://github.com/uNetworking/uWebSockets.js) - the Node.js bindings to µWebSockets, one of the most efficient web servers available

## Build instructions

Node.js 10.x or 11.x is required.

```sh
npm install
npm run build
```

## Run instructions

```sh
./bin/wt-tracker [config.json]
```

or

```sh
node dist/run-uws-tracker.js [config.json]
```

or

```sh
npm start [config.json]
```

## Configuration

See [config.json](sample/config.json)
