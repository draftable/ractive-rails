ractive-rails
=============

### Server side

In your `Gemfile`:

```ruby
gem 'ractive-rails', github: 'Ziplist/ractive-rails'
```

You can choose from the following Ractive versions:
 * `ractive` -- no support for older browsers; lets you generate Ractive templates in the browser
 * `ractive.runtime` -- no support for older browsers; does not let you generate templates browser-side
 * `ractive-legacy` -- with support for older browsers; lets you generate Ractive templates in the browser
 * `ractive-legacy.runtime` -- with support for older browsers; does not let you generate templates browser-side

Include the desired Ractive distribution in the asset pipeline, along with your view templates:

```javascript
//= require ractive
//= require_tree ./views
```

### Extensions supported

```
template.rac
template.ractive
```

### Client side

```javascript
var template = RactiveTemplates["path/to/your/template"];
```

The templates are compiled, so you only need a `.runtime` distribution if you use only templates compiled by `ractive-rails`.
