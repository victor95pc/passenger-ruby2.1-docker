# Passenger-Rails docker using Tutum
Docker for hosting a Rails production app in Phusion Passenger running Ruby 2.1

## Rails application
Config 'config/database.yml' like:

    production:
        adapter: 'postgresql' %>
        port: <%= ENV['APP_DB_PORT'] || "5432" %>
        database: <%= ENV['APP_DB_DATABASE'] %>
        username: <%= ENV['APP_DB_USERNAME'] %>
        password: <%= ENV['APP_DB_PASSWORD'] %> 

