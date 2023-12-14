# Programming_clues

1. [Decorators](#1)
2. [if __name__ == '__main__'](#2)

 

<a name="1"></a>
## Decorators

In a web application, routes are what we type into the browser to go to different pages. We create these using route decorators. Decorators are a way to add additional functionality to  existing functions. In our case, the app.route decorator below handles all the complicated backend stuff and simply allows us to write a function that returns the information that will be shown on the website for this specific route. 

        from flask import Flask 
        app = Flask(__name__)
        
        @app.route("/") # "/" is the root/home page for our website
        def hello():
            return "<h1>Hello World!</h1>"

<a name="2"></a>
## **if __name__ == '__main__'**

This construct in Python is used to check whether the Python script is being run as **the main program or if it is being imported as a module into another script**. Here's how it works:

When a Python script is executed, **a special built-in variable called __name__ is defined.** If the script is the main program being run, then __name__ is set to '__main__'. If the script is being imported as a module into another script, then __name__ is set to the name of the script/module.

So, the if __name__ == '__main__': block allows you to write code that will only be executed when the script is run directly, not when it's imported as a module.

good link: https://www.youtube.com/watch?v=sugvnHA7ElY

