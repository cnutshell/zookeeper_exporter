# Prometheus ZooKeeper Exporter

An exporter for [Prometheus](http://prometheus.io/) to monitor an [Apache ZooKeeper](http://zookeeper.apache.org/) ensemble.

## Building and Running

    make
    ./zookeeper_exporter

### Modes

zookeeper_exporter can be run in two modes: exhibitor and explicit.

The distinction between 'exhibitor' and 'explicit' is how to specify the zookeeper servers.

- The default mode is 'explicit', in which the list of zookeeper servers are specified via command line args.

- In the other mode 'exhibitor', zookeeper servers are discovered by querying certain url from some nodes which are also specified by the same command lines args.

To enable 'exhibitor' mode, use the `-exporter.discovery.exhibitor` flag.

