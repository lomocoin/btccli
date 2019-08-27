Bitcoin cli wrapper
----

- Start and stop `bitcoind` from golang.
- Using go to wrap bitcoin cli.

Useful for integreting bitcoin to tests.

See [bitcoin-core-apis](https://bitcoin.org/en/developer-reference#bitcoin-core-apis)

Zero dependency.

## Currently not support windows
Im developing under macOS and linux, not enough time to deal with windows.

## How to use?
- env variable `BITCOIN_BIN_PATH` to your [bitcoin bin] path (see init.go
- `init.go`
- `func.go`
- other funcs normally start with name which same as file preffix (eg:func in `cli_wrap.go` usually like cliXxx)

Notice:
- Some behaviors may be effected by your local bitcoin.conf.


## TODO
- add PSBT support， https://github.com/bitcoin/bitcoin/blob/master/doc/psbt.md

## versions
Im considering keep same as bitcoincore version, currently 0.18.0.


## LiCENSE
BSD 3-Clause License

