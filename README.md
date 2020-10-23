# docker-openvpn
docker openvpn server

# build
docker build -t fazelit/openvpn -f DockeFile ./

# run
docker run -it -v $(pwd)/openvpn:/etc/openvpn/ -v $(pwd)/root/:/root --name openvpn --device=/dev/net/tun -p 1194:1194  fazelit/openvpn 

# run admin openvpn and install
./openvpn-install.sh

# ovpn file in root directory