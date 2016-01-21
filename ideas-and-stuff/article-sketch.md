
Revealing module pattern


var book = {
  title: "Gates of Fire",
  logTitle: function() {
    console.log(title)
  },
  setTitle: function(newTitle) {
    this.title = newTitle;
  }
};


When you have typical Object literal pattern, you don't want users to directly change object properties, in this case title of the book. The property itself will be changed, but it's not going to be rendered (updated) anywhere in your application. The only way you want users to access these properties is with logTitle and setTitle methods.

The pattern you can use instead of Object literal is Revealing module pattern. Instead of object we use function to wrap our functions and properties:

var Module = (function() {
  ...
})();

This is called immediately invoked function expression of IIFE. It creates new scope and adds the concept of privacy. Everything inside your module is now private and it can't be accessible outside the function, unless otherwise specified.
Private scope is important because we can protect our sensitive data, but also avoid naming conflicts If you have all your functionality in the same file or not locally scoped these naming collisions can become nightmare.

Here is an example of a revealing module structure:

var Module = (function() {

  var title = "Stardust",
      author = "Neil Gaiman",
      genre = "Fantasy";

  var getAuthor = function () {
    return author;
  };

  var setGenre = function(gnr) {
    genre = gnr;
  };

  return {
    getAuthor: getAuthor
  };

})();

Like this, we define all our functions and variables in the private scope and return an object with chosen parts of our module that we want to reveal as public - our API. Like this, we make it really clear at the end of each module which parts of it are available to outside world.
To access our API from another module we simply prefix our exposed methods with the module name, exactly like Object literal:

Module.getAuthor();

To distinguish between private and public methods, you can follow the private naming convenction - simply add undersore (_) before the name of the method you don't want to expose.

  var _privateMethod = function () {
    // private
  };