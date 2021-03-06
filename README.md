## Update to DIN Setup Script

Modified script from https://sinovate.io/downloads/sin_install_vps_noroot.sh

I had some problems for update my VPS to the new version.

The problem may be caused because the script install folders, daemon, etc in the $HOME and the new daemon works in the /root.

You can check the changes from the original script in [CHANGES.md](https://github.com/israelps95/Sinovate/blob/main/CHANGES.md)

## What to do for update my node to DIN?

### In the local wallet:
-You must save the infinitynodeprivkey from the infinitenode.conf

### In the VPS:
Login to your infinity user.

```
su
```
```
bash
```
```
wget https://raw.githubusercontent.com/israelps95/Sinovate/main/update.sh
```
```
chmod +x update.sh
```
```
sudo ./update.sh
``` 

You will be asked by your infinitynode user, write it.

![Image](https://github.com/israelps95/Sinovate/blob/main/img_11.jpg)

Here, paste your infinitynodeprivkey saved in "In the local wallet:".

Wait till it finishes.

After it finishes, you can check the status of the synchronization with
```
watch -n 5 '~/sin-cli getblockcount && ~/sin-cli masternode status && ~/sin-cli mnsync status'
```
```
cd /root
```
Then, you can jump here: https://docs.sinovate.io/#/double_run_guide

Follow in 
```
:~$ ./sin-cli infinitynode keypair
```


## Donations
You can donate SIN in: SiukZP176rkgk4xBa3MvnjpRp1gcUzbrcL
