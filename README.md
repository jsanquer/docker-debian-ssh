
# docker-debian-ssh
A dockerfile for sshd on debian


# build
docker build -t jsanquer/debian-ssh:v1 .


# run
SSH_KEY=$(base64 --wrap=0 ~/.ssh/id_rsa.pub) docker run -i -t -p 2222:22 -e SSH_KEY jsanquer/debian-ssh:v1

# connect
connect as root

