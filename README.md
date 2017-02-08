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
