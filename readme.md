# Dat awesome [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

[<img src="http://datproject.github.io/design/downloads/dat-data-logo.png" align="right" width="140">](https://datproject.org)

> A curated list of the [Dat Project](https://datproject.org) ecosystem.

*Please read the [contribution guidelines](contributing.md) before contributing.*

Want to learn more? Check out:

* [docs.datproject.org](https://docs.datproject.org/)
* [dat whitepaper](https://datproject.org/paper)
* [chat.datproject.org](http://chat.datproject.org/)

## Dat Applications

User facing applications for sharing, downloading, and managing dats.

- [dat](https://github.com/datproject/dat) - command line interface for managing dat archives
- [Dat Desktop](https://github.com/datproject/dat-desktop) - desktop app for managing dat archives
- [Beaker Browser](https://beakerbrowser.com/) - a peer-to-peer browser with tools to create and host websites.

### Community Applications

Projects built using Dat to share and transfer data. Open a PR to add your project here!

- [sciencefair](https://github.com/codeforscience/sciencefair) - The open source p2p desktop science library that puts users in control 🔬 📖 http://sciencefair-app.com
- [hyperirc](https://github.com/mafintosh/hyperirc) - bot that mirrors irc channels to a hypercore read-only log
- [soundcloud-archiver](https://github.com/jondashkyle/soundcloud-archiver) - decentralized archives rescue music in case soundcloud shuts down
- [hypervision](https://github.com/mafintosh/hypervision) - watch and broadcast peer-to-peer live video streams
- [hypertweet](https://github.com/joehand/hypertweet) - stream your twitter feed to a hypercore feed
- [dat-photos-app](https://github.com/beakerbrowser/dat-photos-app) - decentralized, peer-to-peer photo sharing app for beaker browser
- [Dat Installer](https://github.com/staltz/dat-installer) - Android mobile app to distribute APK updates

## Using Dat

Modules that help you build things on top of Dat:

### High-Level APIs

High-level APIs that act as glue for many of the Dat modules:

- [dat-node](https://github.com/datproject/dat-node) - Node module for creating Dat applications with distributed file systems.
- [dat-js](https://github.com/datproject/dat-js) - A pure JavaScript browser-friendly api for using dat over webrtc
- [pauls-dat-api](https://github.com/beakerbrowser/pauls-dat-api) - Library of functions that make working with dat / hyperdrive easier.
- [node-dat-archive](https://github.com/beakerbrowser/node-dat-archive) - node api that supports beaker browser DatArchive format, uses `pauls-dat-api`

### Hosting & Dat Management

Tools for hosting Dats, managing sets of Dats, etc.

- [hypercore-archiver](https://github.com/mafintosh/hypercore-archiver) - archiver peer that backs up multiple hypercore / hyperdrive feeds to disk
- [hypercloud](https://github.com/datprotocol/hypercloud) - p2p + ☁
- [hashbase](https://github.com/beakerbrowser/hashbase) - hosting for the peer-to-peer web
- [dat-now](https://github.com/joehand/dat-now) - publish live syncing and versioned websites, files or whatever to `now.sh` instantly
- [dat-share-all](https://github.com/frando/dat-share-all) - quickly share all dats located in a folder from the command-line

Utilities for `hypercore-archiver`:

- [hypercore-archiver-bot](https://github.com/mafintosh/hypercore-archiver-bot) - IRC bot that provides an interface to `hypercore-archiver`
- [hypercore-archiver-ws](https://github.com/joehand/hypercore-archiver-ws) - websocket server for hypercore-archiver

Dat project runs a registry at datproject.org. We use these tools to manage our dats:

- [dat-registry-api](https://github.com/datproject/dat-registry-api) - account registry api for dat archives with user accounts, uses `township`
- [dat-registry-client](https://github.com/datproject/dat-registry-client) - client for registry api for user registration, login and publishing

#### Managing & Aggregating Dats

- [multidat](https://github.com/datproject/multidat) - manage dat archives in multiple locations, uses a dat factory, based on `multidrive`
- [multidrive](https://github.com/datproject/multidrive) - manage multiple hyperdrive archives located anywhere on the filesystem
- [dat-pki](https://github.com/jayrbolton/dat-pki) - A public key infrastructure with many encryption utilities for Dat filesharing
- [injestdb](https://github.com/beakerbrowser/injestdb) - decentralized table/records-based database with sql-like behaviour, uses `node-dat-archive`

#### Http Hosting

- [hyperdrive-http](https://github.com/joehand/hyperdrive-http) - serve hyperdrive archives over http
- [dathttpd](https://github.com/beakerbrowser/dathttpd) - A Web server for Dat and HTTPS, with zero-config TLS.

### Dat Link Utilties

Resolving, parsing, encoding dat links.

- [dat-dns](https://github.com/datprotocol/dat-dns) - issue dns lookups for dat archives using https requests to a target host
- [dat-link-resolve](https://github.com/joehand/dat-link-resolve) - resolve dat url's, links to a dat key using common methods, uses `dat-dns`
- [parse-dat-url](https://github.com/pfrazee/parse-dat-url) - node's `url.parse` updated to support versioned dat url's
- [dat-encoding](https://github.com/juliangruber/dat-encoding) - encoder and decoder that supports the dat url-scheme

### Dat Utilities

Utilities to show information about an existing dat archive.

- [dat-log](https://github.com/joehand/dat-log) - simple cli that lists the history of a dat archive
- [dat-ls](https://github.com/mafintosh/dat-ls) - simple cli that lists all the changes in a dat archive
- [hyperhealth](https://github.com/karissa/hyperhealth) - monitor health of hyperdrive or dat archives, e.g. peer count and peer mirror %
- [hyperdrive-network-speed](https://github.com/joehand/hyperdrive-network-speed) - track upload and download speeds on hyperdrive archives

### File Imports & Exports

- [hyperdrive-import-files](https://github.com/juliangruber/hyperdrive-import-files) - import files and folders into a hyperdrive archive
- [mirror-folder](https://github.com/mafintosh/mirror-folder) - Small module to mirror a folder to another folder. Supports live mode as well.
- [hyperdrive-staging-area](https://github.com/pfrazee/hyperdrive-staging-area) - staging area for uncommited writes that can sync to a hyperdrive archive
- [hyperdrive-to-zip-stream](https://github.com/pfrazee/hyperdrive-to-zip-stream) - export hyperdrive archives as a zip files

### Hypercore Tools

Tools for using hypercore feeds

- [hyperpipe](https://github.com/mafintosh/hyperpipe) - simple cli to pipe and read files into live hypercore feeds


## Dat Core Modules

Things we used to build Dat. Dat tools (CLI, Desktop, dat-node) are opinonated versions of hyperdrive that work well for using facing applications.

- [hyperdrive](https://github.com/mafintosh/hyperdrive) - secure, decentralized peer-to-peer file system on top of hypercore
- [hypercore](https://github.com/mafintosh/hypercore) - decentralized peer-to-peer append-only logs using hypercore protocol

### CLI Utilities

Utilities used in our command line interface

- [dat-doctor](https://github.com/joehand/dat-doctor) - diagnose networking problems for dat, comes bundled with `dat-cli`
- [dat-ignore](https://github.com/joehand/dat-ignore) - check files against `.datignore` before adding to a dat archive
- [dat-json](https://github.com/joehand/dat-json) - read and write `dat.json` files, uses `toiletdb`

### Networking

- [hyperdiscovery](https://github.com/karissa/hyperdiscovery) - join the p2p swarm for hypercore feeds, uses `discovery-swarm`
- [discovery-swarm](https://github.com/mafintosh/discovery-swarm) - discover and connect to peers, uses `discovery-channel`
- [webrtc-swarm](https://github.com/mafintosh/webrtc-swarm) - create a swarm of p2p connections using webrtc and a signalhub
- [dat-swarm-defaults](https://github.com/joehand/dat-swarm-defaults) - default configuration for dns and dht for use with `discovery-swarm`

#### Lower level networking modules

- [discovery-channel](https://github.com/maxogden/discovery-channel) - search discovery networks to find answering peers
- [dns-discovery](https://github.com/mafintosh/dns-discovery) - discover peers using regular- and `multicast-dns`
- [multicast-dns](https://github.com/mafintosh/multicast-dns) - low-level multicast-dns implementation in pure javascript
- [bittorrent-dht](https://github.com/webtorrent/bittorrent-dht) - complete js implementation of DHT peer discovery protocol
- [utp-native](https://github.com/mafintosh/utp-native) - utp protocol implementation, based on `libutp` native bindings
- [signalhub](https://github.com/mafintosh/signalhub) - simple signalling server that can be used to coordinate handshaking with webrtc

### Storage 

- [dat-storage](https://github.com/datproject/dat-storage) - Dat specific storage provider for Hyperdrive
- [dat-secret-storage](https://github.com/datproject/dat-secret-storage) - hyperdrive storage module for dat secret keys

#### Random Access 

Dat relies on random access storage. Any of these modules can be used to provide the storage for a dat archive.

- [abstract-random-access](https://github.com/juliangruber/abstract-random-access) - base class for random access stores
- [multi-random-access](https://github.com/mafintosh/multi-random-access) - combine multiple `abstract-random-access` stores into a single one

The following are specific implementations of abstract-random-access:

- [random-access-file](https://github.com/mafintosh/random-access-file) - continuous reading / writing to files using random offset and lengths
- [random-access-memory](https://github.com/mafintosh/random-access-memory) - same as `random-access-file` but maintains data in memory
- [random-access-page-files](https://github.com/mafintosh/random-access-page-files) - backend writing to fixed size page files, useful for sparse data
- [dat-http](https://github.com/datproject/dat-http) - http transport and storage provider for dat archives
- [random-access-idb](https://github.com/substack/random-access-idb) - random-access-compatible indexedDB storage layer

### Other Related Dat Project Modules

More modules from Dat project that are related to Dat but may not be used currently.

- [peer-network](https://github.com/mafintosh/peer-network) - create internet-accessible servers/clients listening on names, not hostnames
- [hyperdht](https://github.com/mafintosh/hyperdht) - DHT that supports peer discovery and distributed hole punching

## Dat Project Organization Stuff

- [datproject.org](https://github.com/datproject/datproject.org) - datproject.org on github
- [discussions](https://github.com/datproject/discussions/issues) - general dat project discussion, ideas, feature requests
- [styleguide](https://github.com/datproject/design) - styleguide and visual assets for the dat project
- [dat-elements](https://github.com/datproject/dat-elements) - reusable ui elements for dat-based apps, such as loader, sprite, icon
- [dat-colors](https://github.com/kriesse/dat-colors) - css color definitions that match dat styleguide
- [dat-icons](https://github.com/kriesse/dat-icons) - svg icon definitions that match dat styleguide
- [dat.json specification](https://github.com/juliangruber/dat.json) - specification of the dat.json metadata format

## Outdated

Modules that are currently outdated. We released a major breaking change (hypercore v6, hyperdrive v9) in May 2017. This change included major speed and storage improvements. These modules need to be updated to support the new API.

If you want to update one of these, we are happy to help you choose one depending on your interests and what may still be useful.

- [dat.haus](https://github.com/juliangruber/dat.haus) - dat + http + unix, the composable http api to the dat network
- [hyperfeed](https://github.com/poga/hyperfeed) - publish decentralized rss, atom or rdf feeds, based on `hyperdrive` and `feed`
- [normcore](https://github.com/yoshuawuyts/normcore) - no-config distributed streams using `hypercore`
- [github-to-hypercore](https://github.com/yoshuawuyts/github-to-hypercore) - stream github event feeds into hypercore feeds, uses `normcore`
- [hyperspark](https://github.com/poga/hyperspark) - decentralized data processing platform for dat archives, inspired by `spark`
- [hypercore-index](https://github.com/juliangruber/hypercore-index) - linear asynchronous stateful indexing of a hypercore feed
- [hyperdrive-protocol](https://github.com/juliangruber/hyperdrive-encoding) -  message encoding used by `hyperdrive`
- [hyperdrive-http-server](https://github.com/mafintosh/hyperdrive-http-server) - small cli to serve hyperdrive archives over http
- [dat-publish](https://github.com/joehand/hyperdrive-http) - small cli to publish dat archives to a `hyperdrive-http` or `dat-archiver` server
- [dat-push](https://github.com/joehand/dat-push) - small cli for pushing files to a `dat-archiver` or `dat-publish` server
- [dat-backup](https://github.com/joehand/dat-backup) - backup a dat archive as a single file to local storage and retain full history
- [archiver-server](https://github.com/joehand/archiver-server) - serve `hypercore-archiver` feeds over the dat network and http, uses `discovery-swarm`
- [archiver-api](https://github.com/joehand/archiver-api) - simple rest api for accessing `hypercore-archiver` peers
- [hyperdrive-ln](https://github.com/poga/hyperdrive-ln) - create symbolic links between hyperdrive archives
- [hyperdrive-multiwriter](https://github.com/substack/hyperdrive-multiwriter) - present a bundle of hyperdrive archives together as a multi-writer view
- [hyperdrive-named-archives](https://github.com/substack/hyperdrive-named-archives) - create hyperdrive archives that store and load link keys from names
- [git-dat](https://github.com/substack/git-dat) - git plugin to use dat archives as remotes for a git repository
- [jawn](https://github.com/CfABrigadePhiladelphia/jawn) - distributed version control for tabular data, based on `hypercore`
- [dat-archiver](https://github.com/maxogden/dat-archiver) - archiver peer that backs up dat archives, based on `hypercore-archiver`
- [hyperdrive-stats](https://github.com/juliangruber/hyperdrive-stats) - live and persistent statistics tracker for hyperdrive archives
- [hyperdrive-stats-server](https://github.com/karissa/hypercore-stats-server) - server for sending hypercore / hyperdrive stats over server-side events
- [hyperdrive-stats-ui](https://github.com/mafintosh/hypercore-stats-ui) - html-based user interface to `hypercore-stats-server`
- [zip-to-hyperdrive](https://github.com/karissa/zip-to-hyperdrive) - import contents of a zip archive into a hyperdrive archive
- [url-dat](https://github.com/joehand/url-dat) - import files from http url's into a hyperdrive archive, uses `tar-dat`
- [tar-dat](https://github.com/joehand/tar-dat) - stream tar files into a hyperdrive archive
- [hyperdrive-duplicate](https://github.com/joehand/hyperdrive-duplicate) - check if a file is a duplicate to a hyperdrive archive entry

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the Dat team, and contributors have waived all copyright and related or neighboring rights to this work.
