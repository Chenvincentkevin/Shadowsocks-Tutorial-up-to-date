# Shadowsocks-Tutorial-up-to-date
for Linux, Bash command
Up to date Shadowsocks Tutorial by ReadyToGo!

download:
wget https://github.com/shadowsocks/shadowsocks-rust/releases/download/v1.15.3/shadowsocks-v1.15.3.x86_64-unknown-linux-musl.tar.xz


unpack:
xz -d shadowsocks-v1.15.3.x86_64-unknown-linux-musl.tar.xz & tar -xf shadowsocks-v1.15.3.x86_64-unknown-linux-musl.tar & rm shadowsocks-v1.15.3.x86_64-unknown-linux-musl.tar


write config file:
printf -- "{\n \"server\":\"0.0.0.0\",\n \"server_port\":8389,\n \"password\":\"private networking! Let's go.\",\n \"method\":\"aes-256-gcm\",\n \"mode\":\"tcp_and_udp\",\n}\n" > ssconfig.json


and then start
./ssserver --config ssconfig.json --daemonize


this tutor is originally created by ReadyToGo! https://online-go.com/player/518241/ReadyToGo!
Thanks to him that I can use shadowsocks client
