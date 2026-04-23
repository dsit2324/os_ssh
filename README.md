# Postup

1) ssh-keygen -t rsa -b 4096
2) lsblk
3) cp /media/usb/id_rsa ~/.ssh/id_rsa
4) chmod 600 ~/.ssh/id_rsa
5) eval "$(ssh-agent -s)" 
   ssh-add ~/.ssh/id_rsa
6) umount /media/usb
   rm ~/.ssh/id_rsa
   ssh-add -d ~/.ssh/id_rsa
