# docker-compose
docker compose task
C:\devops-champs\docker>docker-compose down
[+] Running 3/3
 - Container curlclient    Removed                                                                                 0.0s
 - Container apache        Removed                                                                                 0.0s
 - Network docker_default  Removed                                                                                 0.6s

C:\devops-champs\docker>docker-compose up
[+] Running 3/2
 - Network docker_default  Created                                                                                 0.7s
 - Container apache        Created                                                                                 0.1s
 - Container curlclient    Created                                                                                 0.0s
Attaching to apache, curlclient
apache      | AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.22.0.2. Set the 'ServerName' directive globally to suppress this message
apache      | AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.22.0.2. Set the 'ServerName' directive globally to suppress this message
apache      | [Mon Dec 19 09:58:54.951082 2022] [mpm_event:notice] [pid 1:tid 140204719967552] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
apache      | [Mon Dec 19 09:58:54.951224 2022] [core:notice] [pid 1:tid 140204719967552] AH00094: Command line: 'httpd -D FOREGROUND'
apache      | 172.22.0.3 - - [19/Dec/2022:09:58:55 +0000] "GET / HTTP/1.1" 200 4
curlclient  | pong attempting ping
apache      | 172.22.0.3 - - [19/Dec/2022:09:58:56 +0000] "GET / HTTP/1.1" 200 4
curlclient  | pong attempting ping
apache      | 172.22.0.3 - - [19/Dec/2022:09:58:57 +0000] "GET / HTTP/1.1" 200 4
curlclient  | pong attempting ping
apache      | 172.22.0.3 - - [19/Dec/2022:09:58:58 +0000] "GET / HTTP/1.1" 200 4
curlclient  | pong attempting ping
Gracefully stopping... (press Ctrl+C again to force)
[+] Running 2/2
 - Container curlclient  Stopped                                                                                                                                                                             10.3s
 - Container apache      Stopped                                                                                                                                                                              1.4s
canceled
