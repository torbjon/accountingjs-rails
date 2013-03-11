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

    //= require accounting


Then you can:
  
  // Default usage:
  accounting.formatMoney(12345678); // $12,345,678.00
  
  // European formatting (custom symbol and separators), could also use options object as second param:
  accounting.formatMoney(4999.99, "€", 2, ".", ","); // €4.999,99
  
  // Negative values are formatted nicely, too:
  accounting.formatMoney(-500000, "£ ", 0); // £ -500,000
  
  // Simple `format` string allows control of symbol position [%v = value, %s = symbol]:
  accounting.formatMoney(5318008, { symbol: "GBP",  format: "%v %s" }); // 5,318,008.00 GBP


See the full usage details on the [accounting.js](http://josscrowcroft.github.com/accounting.js/) site.

