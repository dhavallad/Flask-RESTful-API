# Flask-RESTful-API
### Introduction 

This is simple execerise in order to build RESTful API. The small programm is to create server side code to retierve the random qoute and display on the webpage in JSON format.

### Feature


* No installation required


### Required python modules
Flask

### Explanation
`app.py` is main application file. I declared the Flask and jsonify imports from the Flask framework. Next, I import a random module. This will be used for generating random numbers when I'm serving the quotes. Random numbers will be used to select quotes from the ones which we stored in the quotes.py file. Next, I declare a new Flask application and pass an experiment of the current file's name. We define the serve funny quote function, and we are assigning this function to the /api/GetQuote root.

`quotes.py` file return the list of quotes whenever new obejct is create of this class.

### How to run 
Navigate to the app.py file folder and run below command in terminal

```
python app.py
```

If the Flask framework started correctly, then you should see a local host 5000 port opened and the application is listening on this port (See below for output). 

```
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
 * Restarting with stat
 * Debugger is active!
 * Debugger pin code: 236-631-072
```

So, let's go to a browser, and navigate to localhost:5000/api/GetQuote, the root which we mapped our serve quote matter to, then we should get some JSON response back. Every time you refresh the page, you should get different responses.
