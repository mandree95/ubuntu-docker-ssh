# ubuntu-docker-ssh
This Docker image can be used to ssh into a remote machine to execute commands. Example:
```sh
$ eval $(ssh-agent -s)
$ ssh-add <(echo "$SSH_PRIVATE_KEY")
$ ssh -o StrictHostKeyChecking=no ${SSH_USER}@${SSH_SERVER} "<command to execute>"
```