# rjv (Rails Javascript Variables)

rjv is a set of helpers that can inject any variables from rails to your javascript code.

## Usage

Add this code at the bottom of your layout file (before closing body tag).

```ruby
== rjv_tags
```

Now you can inject variables in your views:

```ruby
- set_var 'someVar', 'someValue'
```

In javascript this variable will be available as:

```javascript
console.log(app.vars.someVar)
```

## Copyright

Copyright (c) 2013 Michał Młoźniak.
