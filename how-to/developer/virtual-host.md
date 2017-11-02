# How to set virtua host for XAMPP

```sh
# host(C:\Windows\System32\drivers\etc\hosts) file
127.0.0.1       sample.local
127.0.0.1       anothersample.local
```

```sh
# vhost (D:\xampp\apache\conf\extra\httpd-vhosts.conf) file

<VirtualHost *:80>
    DocumentRoot "D:\xampp\htdocs\sample"
    ServerName sample.local
</VirtualHost>

<VirtualHost *:80>
    DocumentRoot "D:/xampp/htdocs/anothersample"
    ServerName anothersample.local
</VirtualHost>
```