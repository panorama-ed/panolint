# Panolint

[![Build Status](https://github.com/panorama-ed/panolint/workflows/Main/badge.svg)](https://github.com/panorama-ed/panolint/actions)
[![Gem Version](https://img.shields.io/gem/v/panolint.svg)](https://github.com/panorama-ed/panolint)

A small gem containing rules for linting code at Panorama Education.

Please note that the last numbered version is `0.1.6`. All future changes will simply be added to the main branch of this repository. To use the latest version of this gem, please bundle directly from the github source following the installation instructions in this README.

## Installation

Add this line to your application's Gemfile:

```ruby
gem "panolint", git: "https://github.com/panorama-ed/panolint.git", branch: "main"
```

And then execute:

    $ bundle

## Usage

### `brakeman`

You can use `panolint`'s `brakeman` configuration in your project by pointing the `brakeman` run at the configuration file in this repo:

```
$ bundle exec brakeman -c "$(bundle show brakeman)/brakeman.yml"
```

### `rubocop`

You can use `panolint`'s rubocop configuration in your project with the following addition to the top of your project's `.rubocop.yml`:

```
inherit_gem:
  panolint: panolint-rubocop.yml
```

Note that it for this gem in particular in needs to not be a `.rubocop.yml` file because of rubocop's [path relativity](https://github.com/rubocop-hq/rubocop/blob/master/manual/configuration.md#path-relativity).

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`.

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/panorama-ed/panolint. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the Panolint project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/[USERNAME]/panolint/blob/master/CODE_OF_CONDUCT.md).
