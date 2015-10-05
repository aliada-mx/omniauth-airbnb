# Omniauth::Airbnb

Welcome to your new gem! In this directory, you'll find the files you
need to be able to package up your Ruby library into a gem. Put your
Ruby code in the file `lib/omniauth/airbnb`. To experiment with that
code, run `bin/console` for an interactive prompt.

TODO: Delete this and the text above, and describe your gem

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'omniauth-airbnb'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install omniauth-airbnb

## Usage

  Rails.application.config.middleware.use OmniAuth::Builder do
    provider :airbnb, ENV['AIRBNB_CLIENT_ID'], ENV['AIRBNB_CLIENT_SECRET'],
    options: { scope: 'basic_profile_read,email_read,reservations_read,listings_read' }
  end


## Development

After checking out the repo, run `bin/setup` to install dependencies.
Then, run `rake spec` to run the tests. You can also run `bin/console`
for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake
install`. To release a new version, update the version number in
`version.rb`, and then run `bundle exec rake release`, which will create
a git tag for the version, push git commits and tags, and push the
`.gem` file to [rubygems.org](https://rubygems.org).


## License

The gem is available as open source under the terms of the
[MIT License](http://opensource.org/licenses/MIT).

