# https-github.com-NikitasGithub-Deployment-script
RUN THE COMMAND IN NODES:
modprobe br_netfilter
echo 1 > /proc/sys/net/bridge/bridge-nf-call-iptables
echo 1 > /proc/sys/net/ipv4/ip_forward
