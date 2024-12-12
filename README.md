# https-github.com-NikitasGithub-Deployment-script
RUN THE COMMAND IN NODES:
modprobe br_netfilter
echo 1 > /proc/sys/net/bridge/bridge-nf-call-iptables
echo 1 > /proc/sys/net/ipv4/ip_forward

Then run the below command ensuring to change your ip address
kubeadm join 172.31.84.58:6443 --cri-socket unix:///var/run/cri-dockerd.sock --token 0rjtvd.wpy10s66ko6h46ww --discovery-token-ca-cert-hash sha256:b55f871dc7e843f984575f64cdc670bb3947c9d46649765d73ee1259c837dd4a
