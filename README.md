# Friend Finder - Node and Express Servers

### Overview

In this activity, I've built a compatibility-based "FriendFinder" application to match you with your favorite Friends character. As users input their information, more friends are formed. This full-stack site will take in results from your users' surveys, then compare their answers with those from other users. The app will then display the name and picture of the user with the best overall match.

You will use Express to handle routing


### Requirements

1. The survey has 10 questions of my choosing. Each answer is on a scale of 1 to 5 based on how much the user agrees or disagrees with a question.

2. The `server.js` file requires the basic npm packages we've used in class: `express` and `path`.

3. The `htmlRoutes.js` file includes two routes:

   * A GET Route to `/survey` which displays the survey page.
   * A default, catch-all route that leads to `home.html` which displays the home page.

4. The `apiRoutes.js` file contains two routes:

   * A GET route with the url `/api/friends`. This is used to display a JSON of all possible friends.
   * A POST routes `/api/friends`. This is used to handle incoming survey results. This route is also used to handle the compatibility logic.

5. The application's data is saved inside of `app/data/friends.js` as an array of objects. Each of these objects follows the format below.

```json
{
  "name":"Joey",
  "photo":"https://vignette.wikia.nocookie.net/friends/images/f/f5/JoeyTribbiani.jpg/revision/latest?cb=20180424154245",
  "scores":[
      5,
      1,
      4,
      4,
      5,
      1,
      2,
      5,
      4,
      1
    ]
}
```

6. The user's most compatible friend is determined.

7. Once the current user's most compatible friend has been found, the result is displayed as a modal pop-up.
   * The modal display both the name and picture of the closest match.

### Live App

1. Click here to find a friend! https://frozen-inlet-63298.herokuapp.com/
