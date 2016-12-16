# Hotel-APP
Hoel-App displays a list of hotels and allows users to view new hotels from an expia API and post reviews.
IT CURRENTLY DOES NOT WORK.
https://mean-hotel-app.herokuapp.com/

# CREDIT
This app was base off a tutorial authored by Simon Holmes. The tutorial is on hostd on the Udemy Website. 
https://www.udemy.com/the-complete-javascript-developer-mean-stack-zero-to-hero/

The tutorial was a video series on the mean stack. I started doing this tutorial a little after the final project was announced. I followed along and learned quite a few things along the way. The app was supposed to store hotels and reviews. I was going to use Expedia's api to call data about hotels and their locations.

# Things I should have done
var mongoose = require('mongoose');
var dburl = 'mongodb://john:john@ds133418.mlab.com:33418/hotel-database';
var retry = null;
mongoose.connect(dburl);

# Should actually be
var mongoose = require('mongoose');
var gracefulShutdown;
//var dbURI = 'mongodb://localhost/map';
var dbURI = 'mongodb://john:john@ds133378.mlab.com:33378/map-app';
if (process.env.NODE_ENV === 'production') {
    dbURI = process.env.MONGODB_URI;
}

# Shold have requied index.js in app.js
require('./api/data/db.js');
var express = require('express');
var app = express();
var path = require('path');
var bodyParser = require('body-parser');

var routes = require('./api/routes');

# My API service would have been called expedia.sevice.js but I didn't get to make that file.
The backend was my main concern and I ran into errors editing the front-end. This git push was my most dependable version.

# Should have pushed o mlabs
hotel dummy data in hotel-data.json
