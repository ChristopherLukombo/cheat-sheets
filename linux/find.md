# Find

find -type f | less  
find / -type f | less  
find / -type d | less  
find "$PWD/" -name "*.java"  
find . | xargs wc -l  
find . -type f -name 'xa*' | xargs sed -i 's/asd/dsg/g'  
find . -name '<terme à chercher>' | xargs grep '<mot à trouver dans les fichiers>'
find / -name "postgresql.conf"