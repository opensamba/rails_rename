== rails_rename renames the hardcoded app_name massively

This repository holds a sample Rails application that make use of unbuilt Rails engines to deliver its functionality.

== Usage

Inside a rails app directory:

  	$ rake rails:rename[NewAppName]
	OldAppName -> NewAppName, these files will be affected, append 'confirm' to apply
	Rakefile
	app/views/layouts/application.html.erb
	config/application.rb
	config/environment.rb
	config/environments/development.rb
	config/environments/production.rb
	config/environments/test.rb
	config/initializers/secret_token.rb
	config/initializers/session_store.rb
	config/routes.rb
	config.ru
	Current app name is: OldAppName



	$ rake rails:rename[NewAppName,confirm]
	Current app name is: NewAppName

== Install

In Gemfile


	gem 'rails_rename'


	bundle install

== License

Copyright (c) Luigi Maselli

Released under the MIT license. See MIT-LICENSE file for details.