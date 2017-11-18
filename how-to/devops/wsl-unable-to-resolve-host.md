# Problem: WSL unable to resolve hostname for [user]

1. execute `sudo su`, you'll get `sudo: unable to resolve host [machine-name]` message, copy your [machine-name].
2. execute `vi /etc/hosts`
3. edit last line with `127.0.0.1 localhost [machine-name]`
