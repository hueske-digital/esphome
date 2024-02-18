## Example caddy host

```
https://esphome.home.yourdomain.de {

    # import logging
    import internal
    import tls
    import compression
    import header

    handle @internal {
        reverse_proxy esphome-app-1:6052
    }
    respond 403
}
```