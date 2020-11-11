## Update to DIN Setup Script

Modified script from https://sinovate.io/downloads/sin_install_vps_noroot.sh

I had some problems for update my VPS to the new version.

The problem may be caused because the script install folders, daemon, etc in the $HOME and the new daemon works in the /root.

## What to do for update my node to DIN?

### In the local wallet:
-You must save the infinitynodeprivkey from the infinitenode.conf

### In the VPS:

```
wget https://raw.githubusercontent.com/israelps95/Sinovate/main/update.sh
```
```
chmod +x update.sh
```
```
sudo ./update.sh
```
![Test Image 4](https://github.com/tograh/testrepository/3DTest.png)
