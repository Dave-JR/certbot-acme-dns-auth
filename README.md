# certbot-acme-dns-auth
certbot manual-auth-hook

$ sudo wget -P /etc/letsencrypt/acme-dns-auth.py https://raw.githubusercontent.com/Dave-JR/certbot-acme-dns-auth/main/acme-dns-auth.py
$ sudo chmod +x /etc/letsencrypt/acme-dns-auth.py

$ sudo certbot certonly --manual --manual-auth-hook /etc/letsencrypt/acme-dns-auth.py --preferred-challenges dns --debug-challenges -d \*.your-domain -d your-domain
