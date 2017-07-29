# Dat awesome [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

[<img src="http://datproject.github.io/design/downloads/dat-data-logo.png" align="right" width="140">](https://datproject.org)

> A curated list of the [Dat Project](https://datproject.org) ecosystem.

*Please read the [contribution guidelines](contributing.md) before contributing.*

[![#dat IRC channel on freenode](https://img.shields.io/badge/irc%20channel-%23dat%20on%20freenode-blue.svg)](http://webchat.freenode.net/?channels=dat)
[![datproject/discussions](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/datproject/discussions?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)


## Technology

- [dat whitepaper](https://datproject.org/paper) - whitepaper 'dat - distributed dataset synchronization And versioning' (pdf)
- [how dat works](https://github.com/datproject/docs/blob/master/docs/how-dat-works.md) - high-level tecnical explanation of how dat works
- [how hypercore works](https://github.com/datproject/docs/blob/master/docs/hyperdrive_spec.md) - in-depth technical explanation of hypercore and hyperdrive
- [dat.json](https://github.com/juliangruber/dat.json) - specification for the dat.json meta format

## Ecosystem

The dat ecosystem consists of many modules provided by the dat project and by the community. The dat project modules are marked:<br>
&nbsp;&nbsp;:small_orange_diamond: = core modules which the dat technology is built on<br>
&nbsp;&nbsp;:small_blue_diamond: = additional modules to be used in dat-based decentralized apps<br>
&nbsp;&nbsp;:small_red_triangle: = important external modules the dat technology is built on

### Top-level

&nbsp;&nbsp;:small_orange_diamond: [dat-node](https://github.com/datproject/dat-node) - node api to the dat framework<br>
&nbsp;&nbsp;:small_orange_diamond: [dat-js](https://github.com/datproject/dat-js) - browser-based api to the dat framework<br>
&nbsp;&nbsp;:small_orange_diamond: [dat-cli](https://github.com/datproject/dat) - command-line interface for managing dats<br>
&nbsp;&nbsp;:small_orange_diamond: [dat-desktop](https://github.com/datproject/dat-desktop) - desktop app for managing dats<br>
- [test](test.html) Test

Hypercore and hyperdrive are core components for dat wire protocol, file-management, -verification and -sharing

- :small_orange_diamond: [hyperdrive](https://github.com/mafintosh/hyperdrive) - secure, decentralized peer-to-peer file system on top of hypercore
- :small_orange_diamond: [hypercore](https://github.com/mafintosh/hypercore) - decentralized peer-to-peer append-only logs on top of hypercore protocol
- :small_orange_diamond: [hypercore-protocol](https://github.com/mafintosh/hypercore-protocol) - stream implementation of the hypercore protocol

### Streams

- :small_orange_diamond: [merkle-tree-stream](https://github.com/mafintosh/merkle-tree-stream) - construct merkle trees from chunks of incoming data
- :small_blue_diamond: [rabin](https://github.com/datproject/rabin) - node-native addon for rabin fingerprinting of data streams

### Networking

- :small_orange_diamond: [hyperdiscovery](https://github.com/karissa/hyperdiscovery) - join the p2p swarm for hypercore feeds, uses discovery-swarm
- :small_orange_diamond: [discovery-swarm](https://github.com/mafintosh/discovery-swarm) - discover and connect to peers, uses discovery-channel
- :small_red_triangle: [discovery-channel](https://github.com/maxogden/discovery-channel) - search multiple discovery networks and find peers who answer
- :small_red_triangle: [dns-discovery](https://github.com/mafintosh/dns-discovery) - discover peers using regular- and multicast-dns
- :small_red_triangle: [bittorrent-dht](https://github.com/webtorrent/bittorrent-dht) - complete implementation of DHT peer discovery protocol in javaScript
- :small_blue_diamond: [utp-native](https://github.com/mafintosh/utp-native) - utp protocol implementation, based on libutp native bindings

### File Access

- [abstract-random-access](https://github.com/juliangruber/abstract-random-access) - Base class for random access stores, such as random-access-file and  random-access-memory.
- [random-access-file](https://github.com/mafintosh/random-access-file) - Continuous reading or writing to a file using random offsets and lengths
- [random-access-memory](https://github.com/mafintosh/random-access-memory) - Exposes the same interface as random-access-file but instead of writing/reading data to a file it maintains it in memory
- [random-access-page-files](https://github.com/mafintosh/random-access-page-files) - An abstract-random-access backend that writes to fixed size page files instead of a single file. Useful for sparse data.


### Command-line

Besides the main [dat-cli](https://github.com/datproject/dat) there are other command-line tools:

- [dat-ls](https://github.com/mafintosh/dat-ls) - Small program that lists all the changes in a dat
- [hyperhttp-cli](https://github.com/joehand/hyperhttp-cli) - simple CLI tool to view a feed or archive metadata on a local http server.
- [dat-doctor](https://github.com/joehand/dat-doctor) - debug dat networking issues


## Using Archives and Feeds

There are lots of modules that help you use, manage, and track Dat archives or hypercore feeds. We use some of these in the CLI and Desktop application!

 - [multidrive](https://github.com/yoshuawuyts/multidrive) - Manage multiple hyperdrive instances.
 - 📔 [dat-node](https://github.com/datproject/dat-node) - Manage Dat archives on the file system.
 - [dat-api](https://github.com/karissa/dat-api) - A pure JavaScript browser-friendly api for using dat.
 - [normcore](https://github.com/yoshuawuyts/normcore) - No-config distributed streams using hypercore

### Importing & Exporting

 - 📔 [hyperdrive-import-files](https://github.com/juliangruber/hyperdrive-import-files) - Import files and folders into a Hyperdrive.
 - [zip-to-hyperdrive](https://github.com/karissa/zip-to-hyperdrive) - Add files from a zip archive to a hyperdrive archive.
 - [hyperdrive-to-zip-stream](https://github.com/pfrazee/hyperdrive-to-zip-stream) - Create a zipfile from a hyperdrive.
 - [hyperdrive-duplicate](https://github.com/joehand/hyperdrive-duplicate) - Check if a file is a duplicate of a file in hyperdrive.
 - [github-to-hypercore](https://github.com/yoshuawuyts/github-to-hypercore) - Stream a github event feed into a hypercore.
 - [url-dat](https://github.com/joehand/url-dat) - Import files from http urls into a dat.
 - [tar-dat](https://github.com/joehand/tar-dat) - Stream tar files into a Dat.

### Networking

- 📔[hyperdiscovery](https://github.com/karissa/hyperdiscovery) - Join the p2p swarm for a given hyperdrive archive.
 - [hyperdrive-http](https://github.com/joehand/hyperdrive-http) - Share Dats over the web! Add http endpoints to an archive.

### Stats

 - 📔 [hyperdrive-stats](https://github.com/juliangruber/hyperdrive-stats) - Live & persistent stats module for tracking archive progress.
 - [hyperdrive-network-speed](https://github.com/joehand/hyperdrive-network-speed) - Track hyperdrive archive upload and download speeds.

### Misc

 - [dat-encoding](https://github.com/juliangruber/dat-encoding) - Dat's way of encoding and decoding dat links
 - [hypercore-index](https://github.com/juliangruber/hypercore-index) - Linear asynchronous stateful indexing of a hypercore feed
 - [hyperdrive-ln](https://github.com/poga/hyperdrive-ln) - create symbolic link between hyperdrives
 - [https://github.com/substack/hyperdrive-multiwriter](hyperdrive-multiwriter) - present a bundle of hyperdrive archives together as a multi-writer view
 - [hyperdrive-named-archives](https://github.com/substack/hyperdrive-named-archives) - create hyperdrive archives that store and load link keys from names


## Browser Modules

- [dat-elements](https://github.com/datproject/dat-elements) - UI elements for Dat
- [hyperdrive-ui](https://github.com/karissa/hyperdrive-ui) - Render a hyperdrive in the browser.


## Archiving, Backup, Dat Servers

- [dat.haus](https://github.com/juliangruber/dat.haus) - The composable HTTP API to the dat network
- [hypercore-archiver](https://github.com/mafintosh/hypercore-archiver) - A hypercore peer that will backup multiple hypercores/hyperdrives efficiently to disk.
- [hypercore-archiver-bot](https://github.com/mafintosh/hypercore-archiver-bot) - IRC bot that is an interface to hypercore-archiver
- [archiver-server](https://github.com/joehand/archiver-server) - Serve archives and feeds from hypercore-archiver over discovery-swarm and HTTP
- [archiver-api](https://github.com/joehand/archiver-api) - rest API for hypercore-archiver.
- [dat-archiver](https://github.com/maxogden/dat-archiver) - a Dat archiving server that you can push data to over the Dat network


## Built with Dat

### Science & Academia

- [Science Fair](https://github.com/codeforscience/sciencefair) - Search, collect, read and reuse the scientific literature over Dat
- [Project Svalbard](https://github.com/datproject/svalbard) - a distributed scientific data archiving network

### Data Processing

- [hyperspark](https://github.com/poga/hyperspark) - Hyperspark is a decentralized data processing tool for Dat. Inspired by Spark.
- [jawn](https://github.com/CfABrigadePhiladelphia/jawn) - Git for Tabular Data.

### Web & Development

- [Beaker Browser](https://beakerbrowser.com/) - A Web Browser that surfs Dats.
- [hyperfeed](https://github.com/poga/hyperfeed) - A self-archiving P2P live feed. You can convert any RSS/ATOM/RDF feed to a P2P live update publishing network.
- [git-dat](https://github.com/substack/git-dat) - git plugin to use dat:// remotes
- [hyperpipe](https://github.com/mafintosh/hyperpipe) - Distributed input/output pipe.


## Organization

- [datproject.org](https://github.com/datproject/website) - datproject.org on github
- [docs.datproject.org](https://github.com/datproject/docs) - docs.datproject.org on github
- [discussions](https://github.com/datproject/discussions/issues) - general dat project discussion, ideas, feature requests
- [styleguide](https://github.com/datproject/design) - styleguide and visual assets for the dat project


## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the Dat team, and contributors have waived all copyright and related or neighboring rights to this work.
