Repo containing Dockerfile to create a busybox based ETCD image. 
Clone of `microbox/etcd` with upgraded version of ETCD, [goUPX](https://github.com/pwaller/goupx) packed.

[![](https://badge.imagelayers.io/anapsix/etcd:v2.3.0.svg)](https://imagelayers.io/?images=anapsix/etcd:v2.3.0)

ETCD Version: 2.3.0

### Usage

    docker run --rm -it -p 4001:4001 -p 7001:7001 -v /var/etcd:/data anapsix/etcd:v2.3.0 --help

Alternatively, you can start a local single node cluster with included script: [start_etcd.sh](https://raw.githubusercontent.com/anapsix/etcd/master/start_etcd.sh)

    ETCD_INITIAL_CLUSTER_STATE=new ./start_etcd.sh

