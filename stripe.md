# Stripe Content Security Policy Rules

Last update: Apr 09, 2019

## script-src
```
https://js.stripe.com
```

## form-action
```
https://hooks.stripe.com/redirect  <-- if you use redirect payment methods like SOFORT\
https://r.girogate.de  <-- if you use SOFORT
```

## connect-src
```
https://api.stripe.com
```

## frame-src
```
https://js.stripe.com
https://hooks.stripe.com
```
