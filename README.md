# ParadropWorkshop

Included is a Vagrantfile that can be used to obtain the Paradrop build setup.

Snap installation on router

Run these commands on vagrant:
```
wget https://paradrop.io/storage/snaps/dnsmasq_2.74_all.snap
wget https://paradrop.io/storage/snaps/hostapd_2.4_all.snap

wget http://pages.cs.wisc.edu/~sejalc/paradrop_0.1.0_all.snap
wget http://pages.cs.wisc.edu/~sejalc/pdinstall_0.1.0_all.snap
```

For deploying snaps:
```
snappy-remote --url=ssh://<ip addr>:22 install dnsmasq_2.74_all.snap
snappy-remote --url=ssh://<ip addr>:22 install hostapd_2.4_all.snap
sudo snappy install docker #run in router
snappy-remote --url=ssh://<ip addr>:22 install paradrop_0.1.0_all.snap
snappy-remote --url=ssh://<ip addr>:22 install pdinstall_0.1.0_all.snap 
```
