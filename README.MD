To run 

run 

nvram show

put file in jffs/my-script


nvram set script_usbmount=sh /jffs/my-script.sh &

cat << EOF >/jffs/my-script.sh

change usb drive to the currect usb name

sh /tmp/mnt/{USB drive}/myscripts/my_simple_autossh >> /mnt/KIOXIA/myscripts/ssh.log &
EOF