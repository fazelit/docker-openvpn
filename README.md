# docker-openvpn
docker openvpn server

# build
dicker build -t fazelit/openvpn 

# run
docker run -it -v <local dir>:/etc/openvpn/ -p 1194:1194  fazelit/openvpn
