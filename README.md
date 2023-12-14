# Programming_clues

1. [Decorators](#1)

 

<a name="1"></a>
Decorators

Routes are what we type into the browser to go to different pages. We create these using route decorators. Decorators are a way to add additional functionality to  existing functions. In our case the app.route decorator below handles all the complicated backend stuff and simply allows us to write a function that returns the information that will be shown on the website for this specific route. 

        from flask import Flask 
        app = Flask(__name__)
        
        @app.route("/") # "/" is the root/home page for our website
        def hello():
            return "<h1>Hello World!</h1>"
