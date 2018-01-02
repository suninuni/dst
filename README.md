# dst

## 依赖

apt update
apt -y install lib32gcc1 libcurl4-gnutls-dev:i386

## 安装 steam

mkdir ~/steamcmd && cd ~/steamcmd

wget https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz
tar -xvzf steamcmd_linux.tar.gz
ln -s /usr/games/steamcmd ~/steamcmd
./steamcmd.sh

## 安装 dst

```
login anonymous
force_install_dir /root/dstserver
app_update 343050 validate
quit
```

## 运行

./dontstarve_dedicated_server_nullrenderer -console -cluster MyClusterName -shard Master
./dontstarve_dedicated_server_nullrenderer -console -cluster MyClusterName -shard Caves
