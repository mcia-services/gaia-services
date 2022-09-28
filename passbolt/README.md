# Passbolt

Webpage for Passbolt: https://www.passbolt.com/

# Generation of the admin user

```bash
$ docker-compose exec passbolt su -m -c "/usr/share/php/passbolt/bin/cake \
                                passbolt register_user \
                                -u <your@email.com> \
                                -f <yourname> \
                                -l <surname> \
                                -r admin" -s /bin/sh www-data
```