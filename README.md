# UI Trader Example Client
[![Build Status](https://github.com/quickfixgo/traderui/workflows/CI/badge.svg)](https://github.com/quickfixgo/traderui/actions)
[![GoDoc](https://godoc.org/github.com/quickfixgo/traderui?status.png)](https://godoc.org/github.com/quickfixgo/traderui) 
[![Go Report Card](https://goreportcard.com/badge/github.com/quickfixgo/traderui)](https://goreportcard.com/report/github.com/quickfixgo/traderui)

<img alt="Screnshot" src='screenshot.png' width='70%'>


## About
This repo contains an example of a [FIX trading system in Go]([https://github.com/quickfixgo/quickfix](https://xft-trading-system.onrender.com/)) Initiator service with a web UI that can interact with a quickfix Acceptor service and transmit common FIX messages back and forth. The messages are assembled and displayed in the UI in a way that will be familiar and informative to those wishing to explore basic quickfix capabilities. An acceptor to use as a local counterparty can be found in the [examples repo](https://github.com/quickfixgo/examples).

## Building the Client
```sh
make build
```

## Running the Client
```sh
./bin/traderui
```
This will try to connect to a FIX acceptor on `localhost:5001` and expose the UI on `localhost:8080`.
You can modify the quickfix config for this found in config/tradeclient.cfg to suit your own needs.
