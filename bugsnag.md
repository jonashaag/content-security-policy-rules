# Bugsnag Content Security Policy Rules

Last update: Jun 15, 2023

> Bugsnag provides error reporting libraries for software platforms

## connect-src
```
https://sessions.bugsnag.com/
https://notify.bugsnag.com/
```

## script-src
```
https://d2wy8f7a9ursnm.cloudfront.net/  <-- if bugsnag-js loads from CDN
```

## References

- [Can I use Bugsnag with CSP?](https://docs.bugsnag.com/platforms/javascript/react/faq/#can-i-use-bugsnag-with-csp)
