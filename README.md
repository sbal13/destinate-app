# Destinate

Welcome to Destinate, your last stop for all your trip planning needs!

We're building an app that will eventually allow users to search through destinations and build travel itineraries to create their perfect multi-destination trip!

But we've gotta start somewhere!

## Client

This is what you'll be working on. To get started, we've provided you with an `index.html` file and an `index.js` file, but that's it! Hook it up on your own!

Right now, we need our client to:

1. Display a list of all destinations in neat cards
  - Style as you wish, but they must be cards. For inspiration, look at other travel websites!
2. Display a form to add a destination
  - On submission of this form, we should see a card for that destination appear on the page

## API

In this repository is a `db.json` file containing example data of what we might expect our API to return as JSON. While our backend engineers get started on building our API, you can use this data as a starting point to build us the best front end experience the world has ever seen.

To run the server, simply use json-server: `json-server --watch db.json`

### Endpoints

Here's a list of relevant endpoints for your project:

* `GET /destinations`
  - Returns an array of all existing destinations in the database
  - Sample response: 
    ```js
    [
      {
        "id": 1,
        "name": "Tahiti",
        "image_url": "https://tat.imgix.net/attachments/global/1477683283_original.jpeg?w=640&h=480&fit=crop&crop=entropy&auto=format,enhance&q=60#tatid:1120608",
        "climate": "Tropical",
        "latitude": -17.6509,
        "longitude": -149.4260
      }
    ]
    ```
* `POST /destinations`
  - Sample body:
    ```js
      {
        name: "Somewhere",
        image_url: "http://somewhere.com",
        climate: "something",
        latitude: 33,
        longitude: 92
      }
    ```
  - Sample response:
    ```js
    {
      "id": 1,
      "name": "Somewhere",
      "image_url": "http://somewhere.com",
      "climate": "something",
      "latitude": 33,
      "longitude": 92
    }
    ```
