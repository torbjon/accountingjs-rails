# Accounting.js is a tiny JavaScript library for number, money and currency formatting

Provides an easy-to-use Rails 3.1 asset for [Accounting.js](http://josscrowcroft.github.com/accounting.js/)

# Install

Add it to your Rails application's `Gemfile`:

```ruby
gem 'accountingjs-rails'
```

Then `bundle install`.


# Usage

Add the following to your `app/assets/javascripts/application.js`:

    //= require accountingjs


Then you can:
      
    // formatMoney() - format any number into currency
    accounting.formatMoney(4999.99, "€", 2, ".", ","); // €4.999,99
    
    // formatNumber() - format a number with custom precision and localisation
    accounting.formatNumber(9876543.21, 3, " "); // 9 876 543.210

    // toFixed() - better rounding for floating point numbers
    accounting.toFixed(0.615, 2); // "0.62"

    // unformat() - get a value from any formatted number/currency string
    accounting.unformat("£ 12,345,678.90 GBP"); // 12345678.9


See the full usage details on the [accounting.js](http://josscrowcroft.github.com/accounting.js/) site.

