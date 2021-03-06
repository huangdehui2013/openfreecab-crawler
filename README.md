# Openfreecabs.org crawler

Crawl data from multiple sources for openfreecabs.org

Currently we crawl data from:

1. [Namba Taxi](https://nambataxi.com)
2. [Sms Taxi](http://smstaxi.kg)
3. [Smart Taxi](http://smart-taxi.kg)
4. [EST](https://estaxi.ru)
5. [Pelican](http://pelican.kg)
6. [Jorgo Taxi](http://jorgo.kg)

## Prerequisites

1. [Go](https://golang.org/)
2. [Make](https://www.gnu.org/software/make/)

## Installation

```
mkdir -p $GOPATH/src/github.com/maddevsio/
cd $GOPATH/src/github.com/maddevsio
git clone https://github.com/maddevsio/openfreecab-crawler
cd openfreecab-crawler
make depends
make
```

Or Go way

```
mkdir -p $GOPATH/src/github.com/maddevsio/
cd $GOPATH/src/github.com/maddevsio
git clone https://github.com/maddevsio/openfreecab-crawler
cd openfreecab-crawler
go get -v
go build -v
go install
```

## Configure

```
GLOBAL OPTIONS:
   --storage_root_url value  OpenfreeCabStorage root url (default: "http://localhost:8090") [$OPEN_FREE_CAB_STORAGE_URL]
   --loglevel value          set log level (default: "debug") [$LOG_LEVEL]
   --test_mode               set test mode [$TEST_MODE]
   --update_interval value   Set update interval (default: 15) [$UPDATE_INTERVAL]
   --help, -h                show help
   --version, -v             print the version

```

## Run

```
./openfreecab-crawler
```

## Contributing

Feel free to create issues, sending pull requests.

1. Fork repo
2. Make a changes 
3. Commit
4. Create pull request
