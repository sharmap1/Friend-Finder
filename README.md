# Friend-Finder

This is a compatibility-based "FriendFinder" application -- basically a dating app. This full-stack site will take in results from your users' surveys, then compare their answers with those from other users. The app will then display the name and picture of the user with the best overall match.

This app uses Express to handle routing and is deployed on Heroku so other users can fill it out.

Live link: https://hidden-everglades-93295.herokuapp.com/

## Requirements

- Modularity in the form of separate files for server logic, storing of friends, views, and routing
- 10-question survey to assess uniqueness of users
- Use express, body-parser, and path npm packages in the server.js file
- Separate JavaScript files for routing (htmlRoutes.js and apiRoutes.js)
- Appropriate GET and POST routes for serving HTML pages and API callshttps://* murmuring-island-94264.herokuapp.com/
- Separate file for storing friends (friends.js)
- Calculate best match for user once survey is completed and return that match to the user

## Technologies Used

- JavaScript
- jQuery
- node.js
- Express.js
- HTML
- Bootstrap

## Code Explaination

- Our server.js file sets up the Express server, specifying our port number, the npm packages that need to be loaded, and also the routes, which we have externalized
- There are 2 separate HTML files (home.html and survey.html) that serve as the front-end portion of our code; they determine what the user sees (the homepage and the survey, which will also show the resulting best match)
- Our 2 routing files (htmlRoutes.js and apiRoutes.js) determine the back-end logic (based on the request being made, the response that gets sent to the browser); the HTML routes display the survey and the homepage based on the URL that is accessed, and the API routes send back existing content in our server-side data or add new friends
- Best match is calculated by finding the friend with the minimal difference in scores and then sending that friend to the browser as a JSON object
- A modal is then toggled, displaying the the best match to the person who just took the survey
- In essense, this will also be a form of notes that you may later reference weeks later
- Friends are stored as such:
  {
  name: "Johny",
  photo: "https://i.ytimg.com/vi/LH8RJ9Q0X0M/maxresdefault.jpg",
  scores: ["2", "1", "2", "1", "2"]
  },

## History

```
This marks the end of unit 13 where we have learned:
* Configure an Express.js app to handle GET and POST requests
* Configure an Express.js app to serve static files
* Identify how client-side requests relate to server-side responses
* Parse optional and required parameters when creating server-side routes
* Implement client-side POST requests to submit form data to a server
* Explain and configure middleware to extend the functionality of Express.js

```

## Credits

```
The Coding Bootcamp @ University of Washington

Instructor: Joel Stedman & TA s : Nicklas Aaland, Austin Williams, Katherine Tenhouse
```

## License

[MIT](https://choosealicense.com/licenses/mit/)

## Copyright

Copyright (c) [2019][prasamsha sharma]
