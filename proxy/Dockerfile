FROM ubuntu
RUN apt-get -y update && apt-get -y install wget iptables
WORKDIR /opt
RUN wget -q --show-progress --https-only --timestamping "https://storage.googleapis.com/kubernetes-release/release/v1.9.0/bin/linux/amd64/kube-proxy"
RUN chmod +x /opt/kube-proxy
COPY ./kubeconfig  /opt/kubeconfig
