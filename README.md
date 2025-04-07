# mount_dir


```
lsblk
sudo fdisk /dev/nvme1n1
sudo fdisk -l /dev/nvme1n1
lsblk
sudo fdisk -l /dev/nvme2n1
sudo apt-get update
sudo apt-get install lvm2
lsblk
sudo pvcreate /dev/nvme1n1
sudo pvcreate /dev/nvme2n1
lsblk
sudo vgcreate dataset /dev/nvme1n1 /dev/nvme2n1
df -h
sudo lvcreate -L 3.4T -n dataset_lv dataset
sudo mkfs.ext4 /dev/dataset/dataset_lv
sudo mkdir /mnt/dataset
sudo mount /dev/dataset/dataset_lv /mnt/dataset/
df -h
lsblk
sudo nano /etc/fstab
/dev/space/space_lv /mnt/space ext4 defaults 0 2
cat /etc/fstab
```
