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


    
  # *MUST* come *BEFORE* devise's definitions (below)
  as :user do   
    match '/user/confirmation' => 'milia/confirmations#update', :via => :put, :as => :update_user_confirmation
  end

  devise_for :users, :controllers => { 
    :registrations => "milia/registrations",
    :confirmations => "milia/confirmations",
    :sessions => "milia/sessions", 
    :passwords => "milia/passwords", 
  }


  root :to => "home#index"
    
  # *MUST* come *BEFORE* devise's definitions (below)
  as :user do   
    match '/user/confirmation' => 'milia/confirmations#update', :via => :put, :as => :update_user_confirmation
  end

    
  # *MUST* come *BEFORE* devise's definitions (below)
  as :user do   
    match '/user/confirmation' => 'milia/confirmations#update', :via => :put, :as => :update_user_confirmation
  end

  devise_for :users, :controllers => { 
    :registrations => "milia/registrations",
    :confirmations => "milia/confirmations",
    :sessions => "milia/sessions", 
    :passwords => "milia/passwords", 
  }

  :controllers => { 
    :registrations => "milia/registrations",
    :confirmations => "milia/confirmations",
    :sessions => "milia/sessions", 
    :passwords => "milia/passwords", 
  }

* ...
