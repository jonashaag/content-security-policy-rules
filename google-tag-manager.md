# Google Tag Manager Content Security Policy Rules

Last update: Jun 15, 2023

Contains all of [Google Analytics]({% link google-analytics.md %}), plus:

## script-src
```
'sha256-...'
https://*.googletagmanager.com
https://*.g.doubleclick.net
https://*.googleadservices.com
https://*.google.com
https://*.google.co.uk  <-- Each Google top-level domain (TLD) must be specified individually
```

## img-src
```
https://*.google-analytics.com
https://*.analytics.google.com
https://*.googletagmanager.com
https://*.g.doubleclick.net
https://*.google.com
https://*.google.co.uk  <-- Each Google top-level domain (TLD) must be specified individually
```

## frame-src
```
https://*.googletagmanager.com
https://*.g.doubleclick.net
```

## connect-src
```
https://*.google-analytics.com
https://*.analytics.google.com
https://*.googletagmanager.com
https://*.g.doubleclick.net
https://*.google.com
https://*.google.co.uk  <-- Each Google top-level domain (TLD) must be specified individually
```

## A note about Google Tag Manager Debug Mode

GTM's debug mode is very tricky (if not impossible) to get to work without the use of `unsafe-inline`.
We recommend to either temporarily disable CSP while you're using GTM's debug mode, or to not send
CSP headers to specific (authenticated and authorized!) users -- e.g. by having them log in or provide
a secret URL parameter (like `?csp_disable=jYBHQ5eq866iR3owYewBZjvuVgY7L4`).
