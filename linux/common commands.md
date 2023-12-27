# Common commands

/etc/wsl.conf  
/etc/resolv.conf  
cntlm -v -c cntlm.conf  
ls | xargs rm  
ps aux | awk '{print $2}'
ps xua | awk '(NR > 1) {print $2}'
ps xua | awk '{print $2}' | awk '(NR>1)'
!! previous command  
sudo apt-get update && sudo apt-get upgrade -y
chmod 700 /mnt/dbtemp
chown postgres:postgres /mnt/dbtemp
ln -s /mnt/c/Users/christopher win_home
eval `keychain --agents ssh --eval ~/.ssh/id_rsa.pub`
ls -al /etc/apt/sources.list.d/

curl -X POST -H "Content-Type: application/json" \

 -d '{"name": "Item 1"}' \

 [http://localhost:8080/items/](http://localhost:8080/items/)

nvm alias default 20.10.0

nvm use

ipconfig.exe | grep IPv4 | cut -d: -f2