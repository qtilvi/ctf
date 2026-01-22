# Nmap
## Open ports:
    - 22 | OpenSSH 8.2p1 Ubuntu
    - 80 | Apache httpd 2.4.41 Ubuntu
## Gobuster:
`gobuster dir -u http://10.81.139.242/ -w .local/share/wordlists/dirb/directory-list-2.3-medium.txt -x html,css,js,scss,php`
    - assets/
    - robots.txt
    - index.html
    - login.php
    - portal.php
## portal.php:
    - /var/www/html:
        - clue.txt
        - Sup3rS3cretPickl3Ingred.txt
## Credentials:
    - R1ckRul3s | Wubbalubbadubdub: found in comment on index.html; password: found in robots.txt
