# tools

- `docker run theyahya/sherlock exfly` Find usernames across social networks

## generate secret

date +%s | shasum | base64 | head -c 32 ; echo
openssl rand -base64 32
