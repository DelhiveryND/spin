# Spinnaker CLI

Edit pipelines, applications & intents.

# Installation & Configuration

Follow the instructions at [spinnaker.io](https://spinnaker.io/docs/setup/other_config/spin/).

# Development

Get started by reading the [Contributing doc](CONTRIBUTING.md).


# Installation

## MacOSX M1
```
go get -u golang.org/x/sys
GOARCH=arm64 GOOS=darwin CGO_ENABLED=0 LD_VERSION=logisticly-dev go build -ldflags "${LD_VERSION}" .
chmod +x ./spin
sudo cp ./spin /usr/local/bin/spin
```


## MacOSX Intel
```
go get -u golang.org/x/sys
GOARCH=amd64 GOOS=darwin CGO_ENABLED=0 LD_VERSION=logisticly-dev go build -ldflags "${LD_VERSION}" .
chmod +x ./spin
sudo cp ./spin /usr/local/bin/spin
```

## Linux Amd64
```
GOARCH=amd64 GOOS=linux CGO_ENABLED=0 LD_VERSION=logisticly-dev go build -ldflags "${LD_VERSION}" .
chmod +x ./spin
sudo cp ./spin /usr/local/bin/spin
```