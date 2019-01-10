# Website

## Requirements:
* Ruby `5.1` or higher
* MySQL installation
* *Windows Only* Ruby [DevKit `x.x.x`](http://rubyinstaller.org/downloads) (required by nokogiri)

## Setup
* `bundle install`
* Set `api-out` in `avicus.yml` to where you want the classes to go
** *NOTE* There may be additional configuration you can do in the `config` folder
* Ensure the config in `avicus.yml` and `database.yml` is set to your details
* Modify details in `config/application.rb` to your details :)

## How to Test:
* Install required gems with `bundle install`
* Run the `localhost:3000` server via `rails s`

## Running as a server w/ modes
* `rails main` for the website
* `raile api` for an api-only website
* IMPORTANT NOTES: API will only recieve api requests, main will only accept website related requests meaning /api won't work on main and everything else wont work on api
* `-e production` to run in `production` mode
* `-b 0.0.0.0` to bind server to 0.0.0.0
* `-p 80` to run on port 80

## Extra
* Look through config folder for potential assets/other text you need to change
* `app/assets` for logos
* `apps/views` for layout modifications

## Bulding API Java Classes
* Follow setup steps first.
* Run `rake graphql:generate` to generate the classes.
* When the classes are loaded into the IDE, there will be a lot of unneeded imports, simply run Code -> Reformat Code to fix all errors
