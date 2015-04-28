Repo containing Dockerfile to create a buxybox based ETCD image. 
Clone of `microbox/etcd` with upgraded version of ETCD

ETCD Version: 2.0.10
Size: 12.82 MB

### Usage

    docker run --rm -it -p 4001:4001 -p 7001:7001 -v /var/etcd:/data anapsix/etcd:latest --help

Alternativly, you can start a local single node cluster with included script: [start_etcd.sh](https://raw.githubusercontent.com/anapsix/etcd/master/start_etcd.sh)

    ETCD_INITIAL_CLUSTER_STATE=new ./start_etcd.sh

