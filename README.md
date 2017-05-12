# shibboleth-idp

This builds on top of [Unicon/shibboleth-idp](https://github.com/Unicon/shibboleth-idp-dockerized)
to provide a ready to run in a single command container for using in my
CI environments.

```shell
docker build -t shib .

docker run -d --name="runshib" -p 4443:4443 -e JETTY_BROWSER_SSL_KEYSTORE_PASSWORD=password shib
```
