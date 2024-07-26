netstat


netstat -ano | grep -c 8080 *.Established

netstat -an | grep 8080 | grep ESTABLISHED | wc -l

lsof -i |grep -c 9010.*ESTABLISHED

netstat -anop