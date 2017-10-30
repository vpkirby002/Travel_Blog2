# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...



Prefix Verb   URI Pattern                                 Controller#Action
           post_comments GET    /posts/:post_id/comments(.:format)          comments#index
                         POST   /posts/:post_id/comments(.:format)          comments#create
        new_post_comment GET    /posts/:post_id/comments/new(.:format)      comments#new
       edit_post_comment GET    /posts/:post_id/comments/:id/edit(.:format) comments#edit
            post_comment GET    /posts/:post_id/comments/:id(.:format)      comments#show
                         PATCH  /posts/:post_id/comments/:id(.:format)      comments#update
                         PUT    /posts/:post_id/comments/:id(.:format)      comments#update
                         DELETE /posts/:post_id/comments/:id(.:format)      comments#destroy
                   posts GET    /posts(.:format)                            posts#index
                         POST   /posts(.:format)                            posts#create
                new_post GET    /posts/new(.:format)                        posts#new
               edit_post GET    /posts/:id/edit(.:format)                   posts#edit
                    post GET    /posts/:id(.:format)                        posts#show
                         PATCH  /posts/:id(.:format)                        posts#update
                         PUT    /posts/:id(.:format)                        posts#update
                         DELETE /posts/:id(.:format)                        posts#destroy
        new_user_session GET    /users/sign_in(.:format)                    devise/sessions#new
            user_session POST   /users/sign_in(.:format)                    devise/sessions#create
    destroy_user_session DELETE /users/sign_out(.:format)                   devise/sessions#destroy
       new_user_password GET    /users/password/new(.:format)               devise/passwords#new
      edit_user_password GET    /users/password/edit(.:format)              devise/passwords#edit
           user_password PATCH  /users/password(.:format)                   devise/passwords#update
                         PUT    /users/password(.:format)                   devise/passwords#update
                         POST   /users/password(.:format)                   devise/passwords#create
cancel_user_registration GET    /users/cancel(.:format)                     devise/registrations#cancel
   new_user_registration GET    /users/sign_up(.:format)                    devise/registrations#new
  edit_user_registration GET    /users/edit(.:format)                       devise/registrations#edit
       user_registration PATCH  /users(.:format)                            devise/registrations#update
                         PUT    /users(.:format)                            devise/registrations#update
                         DELETE /users(.:format)                            devise/registrations#destroy
                         POST   /users(.:format)                            devise/registrations#create
                         GET    /posts(.:format)                            posts#index
                         POST   /posts(.:format)                            posts#create
                         GET    /posts/new(.:format)                        posts#new
                         GET    /posts/:id/edit(.:format)                   posts#edit
                         GET    /posts/:id(.:format)                        posts#show
                         PATCH  /posts/:id(.:format)                        posts#update
                         PUT    /posts/:id(.:format)                        posts#update
                         DELETE /posts/:id(.:format)                        posts#destroy
                    root GET    /                                           posts#index
