# Stripe Content Security Policy Rules

Last update: Jun 15, 2023

## script-src
```
https://js.stripe.com
https://connect-js.stripe.com
https://checkout.stripe.com
```

## form-action
```
https://hooks.stripe.com/redirect  <-- if you use redirect payment methods like SOFORT
https://r.girogate.de  <-- if you use SOFORT
```

## connect-src
```
https://api.stripe.com
https://checkout.stripe.com
```

## frame-src
```
https://js.stripe.com
https://connect-js.stripe.com
https://hooks.stripe.com
https://checkout.stripe.com
https://b.stripecdn.com
```

## img-src
```
https://*.stripe.com
```