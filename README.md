# README

rails new ac
cd ac
rails g controller rooms show
rails g model message content: text
rails db:migrate
(add root route to rooms#show)
(define rooms controller methods)
(define show.html.erb)
(create app/views/message folder and _message.html.erb)
rails g channel room speak
(add ActionCable route)
(update app/assets/javascripts/channels/room.coffee)
(update app/channels/room_channel.rb)
(update message model to start a job after message creation)
rails g job BroadcastMessage
(define BroadcastMessage job)
(add devise to Gemfile)
bundle
rails g devise:install
rails g devise User
rails g migration AddUserToMessages user:references:index
rails db:migrate
