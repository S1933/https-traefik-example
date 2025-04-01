Hello World with Traefik and HTTPS
==================================

SETUP INSTRUCTIONS:

1. Create letsencrypt directory and file:
   mkdir -p letsencrypt
   touch letsencrypt/acme.json
   chmod 600 letsencrypt/acme.json

2. Start the application:
   docker-compose up -d

ACCESS:
- Website: https://s1933.ovh
- Traefik Dashboard: http://localhost:8080

```
PROJECT FILES:
.
├── docker-compose.yml
├── Dockerfile
├── index.html
├── letsencrypt/
│   └── acme.json
└── README.txt
```

IMPORTANT:
* letsencrypt/acme.json must have 600 permissions
* HTTP automatically redirects to HTTPS