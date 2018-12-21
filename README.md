# Website

## Requirements:
* Ruby `5.1` or higher
* MySQL installation
* *Windows Only* Ruby [DevKit `x.x.x`](http://rubyinstaller.org/downloads) (required by nokogiri)

## Bulding API Java Classes
* `bundle install`
* Set `api-out` in `avicus.yml` to where you want the classes to go.
* Ensure the config in `avicus.yml` and `database.yml` is set to your details
* Modify details in `config/application.rb` to your details :)
* Run `rake graphql:generate` to generate the classes.
* When the classes are loaded into the IDE, there will be a lot of unneeded imports, simply run Code -> Reformat Code to fix all errors

## How to Test:
* Install required gems with `bundle install`
* Run the `localhost:3000` server via `rails s`

## Extra
* Look through config folder for potential assets/other text you need to change
* `app/assets` for logos
* `apps/views` for layout modifications
