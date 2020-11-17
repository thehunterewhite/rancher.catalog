## IPSec Networking

Rancher networking plugin using IPsec.

### Open Ports

Traffic to and from hosts require UDP ports `500` and `4500` to be open.

### Changelog - 0.2.4

#### Router, CNI Driver, Connectivity Check [rancher/net:v0.13.13]
* Fixed a Null Pointer Exception problem causing healthcheck issues.
* Fixed issues with erroring out during startup of ipsec.

### Configuration options
* `RANCHER_DEBUG`

#### ipsec

* `IPSEC_REPLAY_WINDOW_SIZE`
* `IPSEC_IKE_SA_REKEY_INTERVAL`
* `IPSEC_CHILD_SA_REKEY_INTERVAL`
* `RANCHER_IPSEC_PSK`

#### cni-driver

* `DOCKER_BRIDGE`
* `MTU`
* `SUBNET`
* `SUBNET_START_ADDRESS`
* `SUBNET_END_ADDRESS`
* `RANCHER_HAIRPIN_MODE`
* `RANCHER_PROMISCUOUS_MODE`
* `HOST_PORTS`
* `SUBNET_PREFIX`

#### connectivity-check

* `CONNECTIVITY_CHECK_INTERVAL`
* `PEER_CONNECTION_TIMEOUT`
