# [uberspace-letsencrypt](https://github.com/fnkr/uberspace-letsencrypt)

Automatic certificate issuance, renewal and installation for [Uberspace](https://uberspace.de).

## Features

- Automatic certificate issuance, renewal and installation
- Multiple certificates and multiple domains per certificate possible

## Getting started

**1)** Clone uberspace-letsencrypt
```
git clone https://github.com/fnkr/uberspace-letsencrypt.git ~/bin/letsencrypt
```

**2)** Update `letsencrypt.ini` with your email address

**3)** Update `letsencrypt-service` with your domains

**4)** Setup service
```
uberspace-setup-service letsencrypt ~/bin/letsencrypt/letsencrypt-service
```

**5)** Check the logs
```
$ tail -f ~/service/letsencrypt/log/main/current | tai64nlocal
...
2016-10-16 12:01:04.752194500 certificate is valid.
2016-10-16 12:01:04.754141500 killed temporary webserver...
2016-10-16 12:01:04.872220500 All good! Your new certificate will be live within the next five minutes.
```

## Questions? Bugs? Feedback?

[github.com/fnkr/uberspace-letsencrypt/issues](https://github.com/fnkr/uberspace-letsencrypt/issues)
