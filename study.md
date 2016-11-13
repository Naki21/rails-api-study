# Rails as an API Study

Use your favorite search engine and the provided readings to research and answer
the following questions (no prior knowledge is expected).

In your answers, be sure to cite any relevant sources you consulted in your
search. We ask you to write answers in your own words in order to see how you
process what you've read. Please do not answer with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   We'll use our [rails-api-template](https://github.com/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

## Required Readings

-   [Starting Ruby on Rails: What I Wish I Knew | BetterExplained](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
-   [Intermediate Rails: Understanding Models, Views and Controllers | BetterExplained](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)
-   [The Rails Command Line — Ruby on Rails Guides](http://guides.rubyonrails.org/command_line.html)
-   [Rails Routing from the Outside In — Ruby on Rails Guides](http://guides.rubyonrails.org/routing.html)
-   [Action Controller Overview — Ruby on Rails Guides](http://guides.rubyonrails.org/action_controller_overview.html)

## Define Model Responsiblities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
Modles are ruby classes. The model takes methods passed from the controller and preforms tasks based on the request. The model then passes the information back to the controler which sends the information back to its next location (view, server, etc.. ).
```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
The controler takes information passed to it from the server and determines the appropriate methods to pass to the model or the view and then sends the end result back to the server.
```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md
The router takes incoming url from the server and determines which actions to send which controller.
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
Browser issues a GET request which is sent to the server, the server sends the request to the rails router which parses the url to determine which controller to use for the GET. The controler issues methods to send to the model. The model uses this informtion to interact with the database and sends the relevant information to the controler. The controler then uses this updated information to interact with the view layer. The view layer then sends back the appropriate information back to the controller. The information finally passes all of this back to the server which then sends the relevant response back to the browser. 
```
