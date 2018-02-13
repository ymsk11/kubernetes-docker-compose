FROM ubuntu
RUN apt-get update -y && apt-get install -y wget docker.io
WORKDIR /opt
RUN wget -q --show-progress --https-only --timestamping "https://storage.googleapis.com/kubernetes-release/release/v1.9.0/bin/linux/amd64/kubelet"
RUN chmod +x /opt/kubelet
COPY ./kubeconfig  /opt/kubeconfig
