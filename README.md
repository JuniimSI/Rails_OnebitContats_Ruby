# README

Instalando o ruby 2.6.5

Gem install Bundle

bundle install

rails generate devise:install
rails generate devise User
 
rails g migration addNameToUser name:string
rails db:migrate

rails g migration add_authentication_token_to_users "authentication_token:string{30}:uniq"
rake db:migrate

rails c
User.create(email: 'jrfernandesti@gmail.com', password: 'juno4848')

rails g model Contact name:string email:string phone:string description:text user:references
rails db:migrate