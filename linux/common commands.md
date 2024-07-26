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
find . ! -name '*test*.*'-name '*.xml'-execgrep -i 'ProductReplacement'{} \; -print
ls|while read -r; do echo $REPLY; done
time
ls | xargs -n 1 kubectl kustomize
curl -X POST -H "Content-Type: application/json" \
kill -l
 -d '{"name": "Item 1"}' \
 egrep “dummy|Lorem|text” dummy.txt
pdfgrep Linux LINUX.pdf
watch -n 5 ls
expr 2 + 3
nl
Tcpdump -A
ps -ef
 [http://localhost:8080/items/](http://localhost:8080/items/)
rpm -aq  
sudo dnf remove packet
bash -x your_script.sh
nvm alias default 20.10.0

nvm use

ipconfig.exe | grep IPv4 | cut -d: -f2

sudo tcpdump port 3389
lsof -i :8080

sudo dpkg -i $FILE_PATH
sudo apt-get install -f

sed 's/linux/ubuntu/ig' sed.txt

watch 

Psql -U postgres
ls|while read -r; do echo $REPLY; done
```
for pid in $(ps -ef | grep "some search" | awk '{print $2}'); do kill -9 $pid; done
```

watch tail -n 10 deployment.log
https://linuxhint.com/how-to-add-a-package-repository-to-debian/

crontab -e  
* * * * * date >> /home/ec2-user/date.log

sudo -i -u postgres