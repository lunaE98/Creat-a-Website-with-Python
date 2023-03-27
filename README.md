# Creat-a-Website-with-Python
Creating wbesite with python

Let's creating a website with Python is a great way to develop web applications. Python has several web frameworks that make it easy to create a website. In this tutorial, we'll use Flask, which is a popular web framework that is easy to learn.

Here are the steps we'll follow:

Install Flask
Create a Flask application
Define routes
Create templates
Run the application
Let's get started!

Step 1: Install Flask

The first thing we need to do is install Flask. Open your command prompt or terminal and type the following command:

pip install Flask
Step 2: Create a Flask application

Now that Flask is installed, we can create a new Python file and import Flask.

python
from flask import Flask

app = Flask(__name__)
This code creates a new Flask application.

Step 3: Define routes

Next, we'll define the routes for our website. A route is a URL pattern that the user can navigate to. We'll define two routes: one for the home page and one for an about page.

python
@app.route('/')
def home():
    return 'Hello, World!'

@app.route('/about')
def about():
    return 'About page'
This code defines two routes: the home page ("/") and the about page ("/about"). The home() function returns "Hello, World!" when the user navigates to the home page, and the about() function returns "About page" when the user navigates to the about page.

Step 4: Create templates

Now we need to create templates for our website. Templates are HTML files that Flask uses to render web pages. We'll create two templates: one for the home page and one for the about page.

Create a new folder called "templates" and create two new files: "home.html" and "about.html". Here's the code for "home.html":

html
<!DOCTYPE html>
<html>
<head>
    <title>Home Page</title>
</head>
<body>
    <h1>Welcome to my website!</h1>
</body>
</html>
And here's the code for "about.html":

html
Copy code
<!DOCTYPE html>
<html>
<head>
    <title>About Page</title>
</head>
<body>
    <h1>About me</h1>
    <p>Hello I am the website.</p>
</body>
</html>
Step 5: Run the application

Now we can run our Flask application. Add the following code at the end of your Python file:

python
if __name__ == '__main__':
    app.run(debug=True)
This code tells Flask to run the application in debug mode.

Save your Python file as "app.py" and run it from your command prompt or terminal:

python app.py

Now open your web browser and navigate to "http://localhost:5000/" to see the home page. Navigate to "http://localhost:5000/about" to see the about page.

And that's it! You've just created a simple website with Python and Flask. From here, you can build more complex applications by adding more routes, templates, and functionality.
