FROM ubuntu
RUN apt-get update -y && apt-get install -y wget
WORKDIR /opt
RUN wget -q --show-progress --https-only --timestamping "https://storage.googleapis.com/kubernetes-release/release/v1.9.0/bin/linux/amd64/kube-controller-manager"
RUN chmod +x /opt/kube-controller-manager
