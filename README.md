To run a iperf3 server on the first node:

* docker run -dti -p 5201:5201 lcalcote/container-net-perf-iperf3 -s

To connect a client to the server container on another node:

* docker run -ti --rm lcalcote/container-net-perf -c <server ip-address> -t 300 -P 128
