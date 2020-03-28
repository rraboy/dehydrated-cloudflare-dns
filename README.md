# dehydrated-cloudflare-dns
Let's Encrypt + CloudFlareDNS + Dehydrated

based on https://github.com/rraboy/dehydrated-godaddy-dns

# how to run

```
docker run -e CF_DNS_SERVERS='8.8.8.8 8.8.4.4' -e CF_DEBUG='true' -e CF_EMAIL='<EMAIL>' -e CF_KEY='<APIKEY>' -v /opt/letsencrypt/dehydrated/accounts:/opt/letsencrypt/dehydrated/accounts -v /opt/letsencrypt/dehydrated/chains:/opt/letsencrypt/dehydrated/chains -v /opt/letsencrypt/dehydrated/certs:/opt/letsencrypt/dehydrated/certs -ti --rm rraboy/dehydrated-cloudflare:latest --accept-terms -d <fqdn>
```
