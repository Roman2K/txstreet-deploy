# txstreet-deploy

This repo will eventually contain all the tools and instructions necessary to
self-host an instance of [TxStreet][txstreet] ([open-source][txstreet-source])
anywhere.

[txstreet]: https://txstreet.com
[txstreet-source]: https://github.com/txstreet
[progress-report-issue]: https://github.com/Roman2K/txstreet-deploy/issues/1

## Status

Work in progress.

I will be committing experimental tools, config and instructions as I'm making
progress.

Updates will be posted in the [progress report issue][progress-report-issue].

## Objectives

* Fully functional

* Dockerized services

* As little assumptions about the deployment environment as possible

* Sample `docker-compose.yml` of a full instance

  * Including blockchain nodes

## Docker images

A deployment is made up of services talking to each other:

* bitcoin-node
* litecoin-node
* monero-node
* bitcoin-cash-node
* eth-node
* eth-beacon-node
* txstreet-processor-api
* txstreet-processor-websocket-server
* txstreet-bulk-geth-api
* mongodb
* redis

To each service corresponds a Docker image that can be built from Dockerfiles
under `docker/<service>` (upcoming).

## Credits

Thanks to [@tomx-eth] for making such a neat blockchain visualizer, publishing its
source, writing comprehensive docs, and passing the torch to the community on
the Litecoin Telegram.

## Related resources

- [Awesome TxStreet](https://github.com/Roman2K/awesome-txstreet)

## License

All material in this repository and this GitHub project are licensed under the
[GNU AGPLv3][agplv3].

[@tomx-eth]: https://github.com/tomx-eth
[agplv3]: https://choosealicense.com/licenses/agpl-3.0/
