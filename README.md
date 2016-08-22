# Supercache

Supercache is a totally unobtrusive addon that runs along your Rails application rapidly improving your development time by caching ActiveRecord Queries across requests (unlike ActiveRecord QueryCache which happens only within a single request). This is especially helpful when your local database is located elsewhere and avoids costly DNS lookups for each and every query.

## Installation

Add this line to your application’s Gemfile:

```ruby
gem 'supercache'
```

And mount the dashboard in your `config/routes.rb`:

```ruby
mount Supercache::Engine, at: "supercache"
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/bragboy/supercache. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

## Scope for Contribution

1. RSpec Integration
2. Travis Integration
3. Code Climate Integration
4. Moving all assets from CDN to the Gem through Vendor
5. Add Caching Support for HTTP Requests
6. Add Exceptions to Caching
