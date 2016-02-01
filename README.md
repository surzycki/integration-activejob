# Tugboat

*Making integration testing headaches with activejob passé*

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'integration-activejob'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install integration-activejob

## Usage

```ruby
expect(JobType).to be_enqueued
expect(JobType).to be_enqueued.with(*args)
expect(JobType).to be_enqueued.to_run_at(time)

expect(JobType).to be_executed
expect(JobType).to be_executed.with(*args)
expect(JobType).to be_executed.to_run_at(time)
```

### Configure


## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/integration-activejob. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

