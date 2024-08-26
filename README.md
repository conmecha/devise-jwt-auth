# Details
This API has been developed with Ruby on Rails while on API-only mode. There are 3 specifically used gems;
 - [devise](https://github.com/heartcombo/devise)
 - [devise-jwt](https://github.com/waiting-for-dev/devise-jwt)
 - [jsonapi-serializer](https://github.com/jsonapi-serializer/jsonapi-serializer) (For more detail about serializing in Rails, check out this [guide](https://medium.com/@maxfpowell/a-quick-intro-to-rails-serializers-b390ced1fce7))

 Endpoints of this API has; login, logout and signup actions. And for an extra help on front-end a provided "current user" route has added to check details of that user. You can use this template for your own projects.

 ### Note: In order to make sure that there are no conflicts with other process on port 3000, this API will work at port 4000. If you'd like to configure the port, please check `config/puma.rb` file.

 # Endpoints
There are 4 different endpoints;
 - **POST /login** => Logins up the user with email and password attributes.
 - **POST /signup** => Signs up the user with email and password attributes.
 - **DELETE /logout** => Logs out the user if there is a session active by that specific user.
 - **GET /current_user** => Gets the current logged in users informations, such as; email, password, created at (in normal format) and created date (in more readable format).

 # Usage

**Note:** In order to use the API, you should already have [**Ruby (3.3.1)**](https://github.com/ruby/ruby) and [**Rails (7.1.3.2 / 7.1.4)**](https://github.com/rails/rails) installed on your instance.

Clone this repo:

 ```
 git clone https://github.com/yercekimsiz/devise-jwt-auth.git
 ```

Install gems for Rails API:
```
bundle install
```

Start the server with Rails CLI:
```
rails server
```

Enjoy the API.