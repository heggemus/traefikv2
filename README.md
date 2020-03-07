# traefikv2
rewrote my blueprints to comply to traefik v2 new syntax

traefik v1: entrypoints -> frontends -> backends

traefik v2: routers -> middlewares -> services

For this to work, you need a working domain, e.g duckdns.org.

Source the following variables before you deploy this stack:

export DOMAIN="<yourdomain>"
  
export EMAIL="<youremail>" # needed for Letsencrypt
  
export USER=admin

export PASSWORD="yourpassword"

export HASHED_PASSWORD=$(openssl passwd -apr1 $PASSWORD)
