## Eat-Da-Burger!
Hungry? Click to devour your favorite burger. Don't like a burger on the menu? Delete it! Don't see what you want? Head to the bottom of the page to add the burger you're craving.

## Motivation
Eat-Da-Burger was designed to demonstrate basic CRUD (Create, Read, Update, Delete) operations.

## Installation
* Fork It
* Clone It
* Open in your terminal or bash and run NPM Install
* Or click [HERE](https://fast-harbor-46897.herokuapp.com/) to run the live demo

## Technologies
* Node.js
* Express
* Handlebars.js

## Code Sample

*Here is a sample of inner workings of the basic CRUD functions:
'''
// Import the ORM to create functions that will interact with the database.
var orm = require("../config/orm.js");

var burger = {
  all: function(cb) {
    orm.all("burgers", function(res) {
      cb(res);
    });
  },
  // The variables cols and vals are arrays.
  create: function(cols, vals, cb) {
    orm.create("burgers", cols, vals, function(res) {
      cb(res);
    });
  },
  update: function(objColVals, condition, cb) {
    orm.update("burgers", objColVals, condition, function(res) {
      cb(res);
    });
  },
  delete: function(condition, cb) {
    orm.delete("burgers", condition, function(res) {
      cb(res);
    });
  }
};

// Export the database functions for the controller (catsController.js).
module.exports = burger;
'''

## Contact
* jlynnraz@gmail.com
* [LinkedIn](https://www.linkedin.com/in/jaimee-razee/)
* [Portfolio](https://jlynnraz.github.io/Portfolio2/)


<img src="https://vignette.wikia.nocookie.net/spongebob/images/1/1c/Goodbye%2C_Krabby_Patty_205.png/revision/latest?cb=20170310020905" data-canonical-src="https://gyazo.com/eb5c5741b6a9a16c692170a41a49c858.png" width="300" height="200" />

