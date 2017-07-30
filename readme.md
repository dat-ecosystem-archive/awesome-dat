# Dat awesome [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

[<img src="http://datproject.github.io/design/downloads/dat-data-logo.png" align="right" width="140">](https://datproject.org)

> A curated list of the [Dat Project](https://datproject.org) ecosystem.

*Please read the [contribution guidelines](contributing.md) before contributing.*

[![#dat IRC channel on freenode](https://img.shields.io/badge/irc%20channel-%23dat%20on%20freenode-blue.svg)](http://webchat.freenode.net/?channels=dat)
[![datproject/discussions](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/datproject/discussions?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

<br>
|&nbsp; [Technology](#technology) &nbsp;|&nbsp; [Documentation](https://docs.datproject.org) :link: &nbsp;|&nbsp; [Ecosystem](#ecosystem) &nbsp;|&nbsp; [Applications](#applications) &nbsp;|&nbsp; [Information](#information) &nbsp;|&nbsp; [Organization](#organization) &nbsp;|

## Technology

- [dat whitepaper](https://datproject.org/paper) - whitepaper 'dat - distributed dataset synchronization And versioning' (pdf)
- [how dat works](https://github.com/datproject/docs/blob/master/docs/how-dat-works.md) - high-level tecnical explanation of how dat works
- [how hypercore works](https://github.com/datproject/docs/blob/master/docs/hyperdrive_spec.md) - in-depth technical explanation of hypercore and hyperdrive
- [dat.json](https://github.com/juliangruber/dat.json) - specification for the dat.json meta format

## Ecosystem

The dat ecosystem consists of many modules provided by dat project and the community:

- [management](#management)
- [streams](#streams)
- [networking](#networking)
- [http / web](#http-web)
- [data access](#file-access)
- [data storage](#data-storage)
- [file exchange](#file-exchange)
- [monitoring](#monitoring)
- [command-line](#command-line)

> Modules are labeled as follows:<br>
> &nbsp;&nbsp;&nbsp;&nbsp;:small_orange_diamond: _core modules which the dat technology is built on_<br>
> &nbsp;&nbsp;&nbsp;&nbsp;:small_blue_diamond: _optional modules provided by the dat project_<br>
> &nbsp;&nbsp;&nbsp;&nbsp;:small_red_triangle: _important external modules the dat technology depends on_<br>
> &nbsp;&nbsp;&nbsp;&nbsp;:black_small_square: _community-contributed ecosystem modules_<br>

### Management

&nbsp;&nbsp;:small_orange_diamond: [dat-node](https://github.com/datproject/dat-node) - node api to the dat framework<br>
&nbsp;&nbsp;:small_blue_diamond: [dat-js](https://github.com/datproject/dat-js) - browser api to the dat framework<br>
&nbsp;&nbsp;:small_blue_diamond: [dat-cli](https://github.com/datproject/dat) - command-line interface for managing dats<br>
&nbsp;&nbsp;:small_blue_diamond: [dat-desktop](https://github.com/datproject/dat-desktop) - desktop app for managing dats<br>

Core components for dat wire protocol, file management, verification and sharing:

&nbsp;&nbsp;:small_orange_diamond: [hyperdrive](https://github.com/mafintosh/hyperdrive) - secure, decentralized peer-to-peer file system on top of hypercore<br>
&nbsp;&nbsp;:small_orange_diamond: [hypercore](https://github.com/mafintosh/hypercore) - decentralized peer-to-peer append-only logs using hypercore protocol<br>

### Streams

&nbsp;&nbsp;:small_orange_diamond: [merkle-tree-stream](https://github.com/mafintosh/merkle-tree-stream) - construct merkle trees from chunks of incoming data<br>
&nbsp;&nbsp;:small_orange_diamond: [hypercore-index](https://github.com/juliangruber/hypercore-index) - linear asynchronous stateful indexing of a hypercore feed<br>
&nbsp;&nbsp;:small_blue_diamond: [rabin](https://github.com/datproject/rabin) - node-native addon for rabin fingerprinting of data streams<br>
&nbsp;&nbsp;:black_small_square: [normcore](https://github.com/yoshuawuyts/normcore) - no-config distributed streams using `hypercore`<br>
&nbsp;&nbsp;:black_small_square: [github-to-hypercore](https://github.com/yoshuawuyts/github-to-hypercore) - stream github event feeds into hypercore feeds, uses `normcore`<br>

### Networking

&nbsp;&nbsp;:small_orange_diamond: [hypercore-protocol](https://github.com/mafintosh/hypercore-protocol) - stream implementation of the hypercore protocol<br>
&nbsp;&nbsp;:small_orange_diamond: [hyperdrive-protocol](https://github.com/juliangruber/hyperdrive-encoding) -  message encoding used by `hyperdrive`<br>
&nbsp;&nbsp;:small_orange_diamond: [dat-encoding](https://github.com/juliangruber/dat-encoding) - encoder and decoder that supports the dat url-scheme<br>
&nbsp;&nbsp;:small_orange_diamond: [hyperdiscovery](https://github.com/karissa/hyperdiscovery) - join the p2p swarm for hypercore feeds, uses `discovery-swarm`<br>
&nbsp;&nbsp;:small_orange_diamond: [discovery-swarm](https://github.com/mafintosh/discovery-swarm) - discover and connect to peers, uses `discovery-channel`<br>
&nbsp;&nbsp;:small_blue_diamond: [utp-native](https://github.com/mafintosh/utp-native) - utp protocol implementation, based on `libutp` native bindings<br>
&nbsp;&nbsp;:small_red_triangle: [discovery-channel](https://github.com/maxogden/discovery-channel) - search discovery networks to find answering peers<br>
&nbsp;&nbsp;:small_red_triangle: [dns-discovery](https://github.com/mafintosh/dns-discovery) - discover peers using regular- and multicast-dns<br>
&nbsp;&nbsp;:small_red_triangle: [bittorrent-dht](https://github.com/webtorrent/bittorrent-dht) - complete js implementation of DHT peer discovery protocol<br>

### HTTP / Web

&nbsp;&nbsp;:small_orange_diamond: [dat-dns](https://github.com/datprotocol/dat-dns) - issue dns lookups for dat archives using https requests to a target host<br>
&nbsp;&nbsp;:small_blue_diamond: [dat-http](https://github.com/datproject/dat-http) - http transport and storage provider for dat archives<br>
&nbsp;&nbsp;:small_blue_diamond: [hyperdrive-http](https://github.com/joehand/hyperdrive-http) - serve hyperdrive archives over http<br>
&nbsp;&nbsp;:small_blue_diamond: [hyperdrive-ui](https://github.com/karissa/hyperdrive-ui) - render hyperdrive archives as html in the browser<br>
&nbsp;&nbsp;:small_blue_diamond: [dat-elements](https://github.com/datproject/dat-elements) - reusable ui elements for dat-based apps, such as loader, sprite, icon<br>
&nbsp;&nbsp;:black_small_square: [dat-colors](https://github.com/kriesse/dat-colors) - css color definitions that match dat styleguide<br>
&nbsp;&nbsp;:black_small_square: [dat-icons](https://github.com/kriesse/dat-icons) - svg icon definitions that match dat styleguide<br>

### Data access

&nbsp;&nbsp;:small_orange_diamond: [abstract-random-access](https://github.com/juliangruber/abstract-random-access) - base class for random access stores<br>
&nbsp;&nbsp;:small_orange_diamond: [multi-random-access](https://github.com/mafintosh/multi-random-access) - combine multiple `abstract-random-access` stores into a single one<br>
&nbsp;&nbsp;:small_blue_diamond: [random-access-file](https://github.com/mafintosh/random-access-file) - continuous reading / writing to files using random offset and lengths<br>
&nbsp;&nbsp;:small_blue_diamond: [random-access-memory](https://github.com/mafintosh/random-access-memory) - same as `random-access-file` but maintains data in memory<br>
&nbsp;&nbsp;:small_blue_diamond: [random-access-page-files](https://github.com/mafintosh/random-access-page-files) - backend writing to fixed size page files, useful for sparse data<br>
&nbsp;&nbsp;:small_orange_diamond: [multidat](https://github.com/datproject/multidat) - manage dat archives in multiple locations, uses a dat factory, based on `multidrive`<br>
&nbsp;&nbsp;:small_orange_diamond: [multidrive](https://github.com/datproject/multidrive) - manage multiple hyperdrive archives located anywhere on the filesystem<br>
&nbsp;&nbsp;:black_small_square: [hyperdrive-ln](https://github.com/poga/hyperdrive-ln) - create symbolic links between hyperdrive archives<br>
&nbsp;&nbsp;:black_small_square: [https://github.com/substack/hyperdrive-multiwriter](hyperdrive-multiwriter) - present a bundle of hyperdrive archives together as a multi-writer view<br>
&nbsp;&nbsp;:black_small_square: [hyperdrive-named-archives](https://github.com/substack/hyperdrive-named-archives) - create hyperdrive archives that store and load link keys from names<br>

### Data storage

&nbsp;&nbsp;:small_orange_diamond: [dat-storage](https://github.com/datproject/dat-storage) - hyperdrive storage provider for dat archives<br>
&nbsp;&nbsp;:small_orange_diamond: [dat-secret-storage](https://github.com/datproject/dat-secret-storage) - hyperdrive storage provider for secret keys<br>

### File exchange

&nbsp;&nbsp;:small_blue_diamond: [hyperdrive-import-files](https://github.com/juliangruber/hyperdrive-import-files) - import files and folders into a hyperdrive archive<br>
&nbsp;&nbsp;:small_blue_diamond: [zip-to-hyperdrive](https://github.com/karissa/zip-to-hyperdrive) - import contents of a zip archive into a hyperdrive archive<br>
&nbsp;&nbsp;:small_blue_diamond: [url-dat](https://github.com/joehand/url-dat) - import files from http url's into a hyperdrive archive, uses `tar-dat`<br>
&nbsp;&nbsp;:small_blue_diamond: [tar-dat](https://github.com/joehand/tar-dat) - stream tar files into a hyperdrive archive<br>
&nbsp;&nbsp;:small_blue_diamond: [hyperdrive-duplicate](https://github.com/joehand/hyperdrive-duplicate) - check if a file is a duplicate to a hyperdrive archive entry<br>
&nbsp;&nbsp;:black_small_square: [hyperdrive-to-zip-stream](https://github.com/pfrazee/hyperdrive-to-zip-stream) - export hyperdrive archives as a zip files<br>

### Monitoring

&nbsp;&nbsp;:small_orange_diamond: [hyperdrive-stats](https://github.com/juliangruber/hyperdrive-stats) - live and persistent statistics tracker for hyperdrive archives<br>
&nbsp;&nbsp;:small_orange_diamond: [hyperdrive-network-speed](https://github.com/joehand/hyperdrive-network-speed) - track upload and download speeds on hyperdrive archives<br>
&nbsp;&nbsp;:small_blue_diamond: [dat-doctor](https://github.com/joehand/dat-doctor) - diagnose networking problems for dat, comes bundled with `dat-cli`<br>
&nbsp;&nbsp;:small_blue_diamond: [dat-ls](https://github.com/mafintosh/dat-ls) - simple cli that lists all the changes in a dat<br>
&nbsp;&nbsp;:small_blue_diamond: [hyperhttp-cli](https://github.com/joehand/hyperhttp-cli) - simple cli to view a feed or archive metadata over http<br>


## Archiving, Backup, Dat Servers

- [hypercore-archiver](https://github.com/mafintosh/hypercore-archiver) - A hypercore peer that will backup multiple hypercores/hyperdrives efficiently to disk.
- [hypercore-archiver-bot](https://github.com/mafintosh/hypercore-archiver-bot) - IRC bot that is an interface to hypercore-archiver
- [archiver-server](https://github.com/joehand/archiver-server) - Serve archives and feeds from hypercore-archiver over discovery-swarm and HTTP
- [archiver-api](https://github.com/joehand/archiver-api) - rest API for hypercore-archiver.
- [dat-archiver](https://github.com/maxogden/dat-archiver) - a Dat archiving server that you can push data to over the Dat network


## Applications

- [dat.haus](https://github.com/juliangruber/dat.haus) - The composable HTTP API to the dat network

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
