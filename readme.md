# **DO NOT REMOVE THIS REPO!**

### This repository maintained to use for Parsclick.

---

# Using the maintained version with composer

1. In your `compose.json` update the `"laravel/cashier-braintree": "3.0"` to `"laravel/cashier-braintree": "dev-master"`

2. Add this in your `composer.json`:

```json
 "repositories": [
    {
        "type": "vcs",
        "url": "https://github.com/hassanazimi/cashier-braintree"
    }
]
```

3. Run `composer update`

# Laravel Cashier - Braintree Edition

[![Build Status](https://travis-ci.org/laravel/cashier-braintree.svg)](https://travis-ci.org/laravel/cashier-braintree)
[![Total Downloads](https://poser.pugx.org/laravel/cashier-braintree/d/total.svg)](https://packagist.org/packages/laravel/cashier-braintree)
[![Latest Stable Version](https://poser.pugx.org/laravel/cashier-braintree/v/stable.svg)](https://packagist.org/packages/laravel/cashier-braintree)
[![Latest Unstable Version](https://poser.pugx.org/laravel/cashier-braintree/v/unstable.svg)](https://packagist.org/packages/laravel/cashier-braintree)
[![License](https://poser.pugx.org/laravel/cashier-braintree/license.svg)](https://packagist.org/packages/laravel/cashier-braintree)

## Introduction

Laravel Cashier Braintree provides an expressive, fluent interface to [Braintree's](https://www.braintreepayments.com/) subscription billing services. It handles almost all of the boilerplate subscription billing code you are dreading writing. In addition to basic subscription management, Cashier Braintree can handle coupons, swapping subscription, cancellation grace periods, and even generate invoice PDFs.

## Testing

You will need to set the following details locally and on your Braintree account in order to run the library's tests.

### Local

#### Environment Variables

    BRAINTREE_MERCHANT_ID=
    BRAINTREE_PUBLIC_KEY=
    BRAINTREE_PRIVATE_KEY=
    BRAINTREE_MODEL=Laravel\Cashier\Tests\User

You can set these variables in the `phpunit.xml.dist` file.

### Braintree

#### Plans

    * Plan ID: monthly-10-1, Price: $10, Billing cycle of every month
    * Plan ID: monthly-10-2, Price: $10, Billing cycle of every month
    * Plan ID: yearly-100-1, Price: $100, Billing cycle of every 12 months

#### Discount

    * Discount ID: coupon-1, Price: $5
    * Discount ID: plan-credit, Price $1

## Official Documentation

Documentation for Cashier Braintree can be found on the [Laravel website](https://laravel.com/docs/5.8/braintree).

## License

Laravel Cashier Braintree is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
