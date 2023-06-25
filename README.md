yum install cifs-utill
mkdir /mnt/treasury-share
# write username and password without space after = sign
vi /etc/treasury-sys-cred
username=
password=

vi /etc/fstab
//10.96.39.121/CommonShare/ /mnt/treasury-share cifs credentials=/etc/treasury-sys-cred,vers=3.0,iocharset=utf8,file_mode=0777,dir_mode=0777,nofail,nodfs 0 0

mount -av
lsblk
fndmnt

then save script
write crontab
