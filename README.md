SpreeOnePageStockManagement
===========================

Demo
-----------------------------------
Try Spree Admin Activity Tracker for Spree 3-4 with direct deployment on Heroku:

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/vinsol-spree-contrib/spree-demo-heroku/tree/spree-one-page-stock-management)


Introduction goes here.

## Installation

1. Add this extension to your Gemfile with this line:
  ```ruby
  gem 'spree_one_page_stock_management', github: 'vinsol-spree-contrib/spree_one_page_stock_management'
  ```

  Also add this to your Gemfile
  ```ruby
  gem 'delayed_job_active_record'
  ```

2. Install the gem using Bundler:
  ```ruby
  bundle install
  ```

3. Copy & run migrations
  ```ruby
  bundle exec rails g spree_one_page_stock_management:install
  ```

4. Restart your server

  If your server was running, restart it so that it can find the assets properly.


## Running

1. Go to general settings under configurations tab in sidebar.
2. Enter the email in Mail to Address field to receive the mail.
3. Go to stock items bar.
4. Update the corresponding stock item as per requirement.

Also you can upload bulk stock item to update by uploading csv file

1. Format for csv can be seen by downloading the sample csv
2. Upload the csv with the following format.
3. Stock items will be updated and failed rows will be informed via mail.

## Testing

First bundle your dependencies, then run `rake`. `rake` will default to building the dummy app if it does not exist, then it will run specs. The dummy app can be regenerated by using `rake test_app`.

```shell
bundle
bundle exec rake
```

When testing your applications integration with this extension you may use it's factories.
Simply add this require statement to your spec_helper:

```ruby
require 'spree_one_page_stock_management/factories'
```


## Contributing

  1. [Fork](https://help.github.com/articles/fork-a-repo) the project
  2. Make one or more well commented and clean commits to the repository. You can make a new branch here if you are modifying more than one part or feature.
  3. Add tests for it. This is important so I don’t break it in a future version unintentionally.
  4. Perform a [pull request](https://help.github.com/articles/using-pull-requests) in github's web interface.


Credits
-------

[![vinsol.com: Ruby on Rails, iOS and Android developers](http://vinsol.com/vin_logo.png "Ruby on Rails, iOS and Android developers")](http://vinsol.com)

Copyright (c) 2017 [vinsol.com](http://vinsol.com "Ruby on Rails, iOS and Android developers"), released under the New MIT License
