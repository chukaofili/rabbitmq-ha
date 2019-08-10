# rabbitmq-ha
Bootstrap RabbitMQ Cluster on Kubernetes

## Pre-requisites

1. Install kubectl
2. Setup a kubernetes cluster

### Repo Setup

* Clone this repo git@github.com:chukaofili/rabbitmq-ha.git
* cd rabbitmq-ha
* chmod 700 ./install.sh

### Prep Work

1. cp [REPO]/cert-manager-install/.env.example [REPO]/cert-manager-install/.env & substitute variables for yours.
2. cp [REPO]/rabbitmq-config/.env.example [REPO]/rabbitmq-config/.env & substitute variables for yours.

### Begin Installation

1. Run ./install.sh
2. Enter **1** to install `helm` or **2** to skip if `helm` is already installed.
3. Enter **1** to install `helm client` or **2** to skip if `helm client` is already installed.
4. Enter **1** to install `ngin-ingress` or **2** to skip if `nginx-ingress` is already installed.
5. Enter **1** to install `cert-manager` or **2** to skip if `cert-manager` is already installed.
6. Enter **1** to install `rabbitmq`
7. After installation, how to access your rabbitmq cluster should be printed in your terminal.
8. Modify your dns records to point your domains (DOMAIN & amqp-DOMAIN) printed on screen to thier repective ips.
