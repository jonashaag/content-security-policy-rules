# Google Tag Manager Content Security Policy Rules

Last update: Aug 21, 2017

All of [Google Analytics]({% link google-analytics.md %}), plus:

## script-src
```
'sha256-...'
https://www.googletagmanager.com/
```

If you use ads:

```
https://googleads.g.doubleclick.net
https://www.google.com/ads/user-list
https://www.google.XYX/ads/user-list
https://bid.g.doubleclick.net
https://www.googleadservices.com
```

## frame-src
```
https://www.googletagmanager.com/ns.html
```

## A note about Google Tag Manager Debug Mode

GTM's debug mode is very tricky (if not impossible) to get to work without the use of `unsafe-inline`.
We recommend to either temporarily disable CSP while you're using GTM's debug mode, or to not send
CSP headers to specific (authenticated and authorized!) users -- e.g. by having them log in or provide
a secret URL parameter (like `?csp_disable=jYBHQ5eq866iR3owYewBZjvuVgY7L4`).
