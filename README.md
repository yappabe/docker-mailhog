# Yappa Mailhog Docker Image

This adds mailhog, which is accessible on port 8025.

## Usage

Add the following to your docker-compose.yml file:

```YAML
mailhog:
    image: yappabe/mailhog
    environment:
        DNSDOCK_ALIAS: mailhog.compass-pools.docker.webfolks.be
```
Next, add this container to your php and nginx container links.

You can now use mailhog as an smtp server, simply use 'mailhog', or whatever you named this container as host on port 1025. No credentials are needed.

## References
* https://github.com/mailhog/MailHog
