# dvlbox.de - Local Testing Domain

## Overview
**dvlbox.de** provides an easy-to-use local testing environment without the need to modify your `hosts` file. All subdomains of `dvlbox.de` automatically resolve to `127.0.0.1` and `::1`, making it perfect for local development and testing.

## How It Works
Instead of manually adding entries in the `hosts` file, you can use `dvlbox.de` for local development:

```
http://newyork.dvlbox.de
http://mysite.dvlbox.de
http://redirecttest.dvlbox.de
http://sub1.sub2.sub3.dvlbox.de
```

Every subdomain of `dvlbox.de` points to `127.0.0.1` or `::1`, ensuring seamless local testing.

## Alternative Test Domains
Other services offer similar functionality:
- [localtest.me](http://localtest.me/)
- [lvh.me](http://lvh.me/)
- [vcap.me](http://vcap.me/)

However, I primarily use [Devilbox](https://github.com/cytopia/devilbox), which integrates perfectly with `dvlbox.de` for local testing.

## Troubleshooting
If `dvlbox.de` does not resolve to `127.0.0.1`, DNS rebinding protection might be enabled on your network. Possible solutions:

1. Check if your router has DNS rebinding protection enabled and allow an exception for `dvlbox.de`.
2. Switch your DNS provider to Cloudflare `1.1.1.1` or Google DNS `8.8.8.8`.
3. Read more about DNS rebinding here:
    - [Wikipedia (DE)](https://de.wikipedia.org/wiki/DNS_Rebinding)
    - [Wikipedia (EN)](https://en.wikipedia.org/wiki/DNS_rebinding)
    - [Fritzbox Configuration Guide](https://avm.de/service/wissensdatenbank/dok/FRITZ-Box-7390/663_DNS-Auflosung-privater-IP-Adressen-nicht-moglich/)

## License
MIT License

