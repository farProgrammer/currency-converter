### Conceptual Exercise

Answer the following questions below:

- What are important differences between Python and JavaScript?
 * Python is an Object-Oriented Programming Language
 * JavaScript is a scripting language, while Python is part of a class of coding languages called “object-oriented” languages.
  
- Given a dictionary like ``{"a": 1, "b": 2}``: , list two ways you
  can try to get a missing key (like "c") *without* your programming
  crashing.
 * dict['c']
 * 
- What is a unit test?
 * A unit test is a way of testing a unit - the smallest piece of code that can be logically isolated in a system. In most programming languages, that is a function, a subroutine, a method or property.
 * 
  
- What is an integration test?
 * INTEGRATION TESTING is a level of software testing where individual units / components are combined and tested as a group.
 * 
     
- What is the role of web application framework, like Flask?
 * Flask is a micro web framework written in Python. Extensions exist for object-relational mappers, form validation, upload handling, various open authentication technologies and several common framework related tools. ... Applications that use the Flask framework include Pinterest and LinkedIn.
 *
 * You can pass information to Flask either as a parameter in a route URL
  (like '/foods/pretzel') or using a URL query param (like
  'foods?type=pretzel'). How might you choose which one is a better fit
  for an application?
 * A parameter in a route URL is best for passing info as a main category for the page that you're looking for
 * 
 * A URL query param is best for passing additional info that simply adds to the page that you're looking for
 * 
- How do you collect data from a URL placeholder parameter using Flask?
 * from flask import request

@app.route(...)
def login():
    username = request.args.get('username')
    password = request.args.get('password')
    
 * 
- How do you collect data from the query string using Flask?
 * To access an individual known param passed in the query string, you can use request. args. get('param')
 * 
- How do you collect data from the body of the request using Flask?
 * request.args: the key/value pairs in the URL query string
request.form: the key/value pairs in the body, from a HTML post form, or JavaScript request that isn't JSON encoded
request.files: the files in the body, which Flask keeps separate from form. HTML forms must use enctype=multipart/form-data or files will not be uploaded.
request.values: combined args and form, preferring args if keys overlap
request.json: parsed JSON data. The request must have the application/json content type, or use request.get_json(force=True) to ignore the content type.
 * 
- What is a cookie and what kinds of things are they commonly used for?
 * Cookies are small text files placed on a user’s computer (or smartphone), which are commonly used to collect personal data.Cookies are used to make the user's web experience faster, convenient and personalised. For example you can select a language to view a website the first time you visit it. When you visit the website again it will save your preference.
 * 
- What is the session object in Flask?
 * n the flask, a session object is used to track the session data which is a dictionary object that contains a key-value pair of the session variables and their associated values. The following syntax is used to set the session variable to a specific value on the server.
 * 
- What does Flask's `jsonify()` do?
 * jsonify() is a helper method provided by Flask to properly return JSON data. jsonify() returns a Response object with the application/json mimetype set.
 * 