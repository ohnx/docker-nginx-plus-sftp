# nginx-homedir

docker + alpine linux + nginx, but nginx is configured to serve files in /home/.../public_html as /~.../

Typical of servers that host web data for lots of users.

Recommended usage is to create a volume (i.e. `docker volume create --name webserver_users`)
and mount that at `/home` on this container, as well as a container with some sort of file host (e.g. sFTP, FTP).
