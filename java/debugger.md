# Debugger

java  -jar -agentlib:jdwp=transport=dt_socket,server=y,suspend=n,address=*:5005 todobackend-0.0.1-SNAPSHOT.jar