#FeedMyCuriosity

## Minimum Viable Product

FeedMyCuriosity is a web application inspired by Feedly that will be built using Ruby on Rails and React.js. By the end of Week 9, this app will, at a minimum, satisfy the following criteria:

- [ ] New account creation, login, and guest/demo login
- [ ] Smooth, bug-free navigation
- [ ] Adequate seed data to demonstrate the site's features
- [ ] The minimally necessary features for a Feedly-inspired site: CRUD collections, displaying the feeds of the user, and providing feeds for the user to choose from
- [ ] Hosting on Heroku
- [ ] CSS styling that is satisfactorily visually appealing
- [ ] A production README, replacing this README

## Product Goals and Priorities
### MVP
- [ ] Create an account (MVP)
- [ ] Log in/ Log out, including as a Guest/Demo User (MVP)
- [ ] Make collections (MVP)
- [ ] Display user's feeds and collections (MVP)
- [ ] Add and remove feeds from collections (MVP)
- [ ] Provide feeds for the user to choose from (MVP)
- [ ] Provides link to go to feed's website (MVP)
- [ ] Feeds display recent articles (MVP)

### Expected Features
- [ ] Feeds show number of hits
- [ ] Categorizes feeds by date
- [ ] Mark article as read once user has clicked on article in feed
- [ ] Displays time the article was posted ( expected feature but not MVP)
- [ ] Able to organize collections
- [ ] Able to search for feeds
- [ ] Have subcategories of feeds
- [ ] Feeds have logos, Users have a profile picture
- [ ] Have a button to save articles to read for later
- [ ] User can hide or save articles

### Bonus Features
- [ ] User can choose how to display the articles of a feed
- [ ] Embed videos for feeds with videos
- [ ] Displays related feeds when displaying articles of a particular feed
- [ ] User can mark all of the articles of a feed as read all at once
- [ ] User can set preferences
- [ ] User can select a theme for sidebar
- [ ] User can share collections through a url

## Design Docs
* [View Wireframes][views]
* [React Components][components]
* [Flux Cycles][flux-cycles]
* [API endpoints][api-endpoints]
* [DB schema][schema]

[views]: ./docs/views.md
[components]: ./docs/components.md
[flux-cycles]: ./docs/flux-cycles.md
[api-endpoints]: ./docs/api-endpoints.md
[schema]: ./docs/schema.md

## Implementation Timeline

### Phase 1: Backend setup and User Authentication (0.5 days)

**Objective:** Functioning rails project with Authentication

- [ ] create new project
- [ ] setup Webpack and Flux scaffold
- [ ] create `User` model
- [ ] authentication
  - [ ] ensure_session_token
  - [ ] reset_session_token
  - [ ] generate session_token
  - [ ] current_user
  - [ ] password=
  - [ ] validations
  - [ ] logout!
  - [ ] login
- [ ] user signup/signin pages
  - [ ] Make views for now, refactor into React Component later
- [ ] blank landing page after sign in
- [ ] seed some users to database

### Phase 2: Feeds Model, API, basic APIUtil, Actions, and STORE (0.5 days)

**Objective** Feeds can be retrieved through the API

- [ ] create `Feed` model
- [ ] seed the database with small amount of rss feeds from websites that provide it
- [ ] Retrieve feeds data by using an FeedAPI (`FeedsController`) to fetch the feed data
- [ ] jBuilder views for parsed data from Feed url using Feedjira gem
- [ ] setup `ApiUtil` to interact with the API
- [ ] test out API interaction in the console
- [ ] setup `FeedStore`, `FeedServerActions`, `FeedClientActions`
    - [ ] write the methods
    - [ ] test the methods

### Phase 3: Frontend Feeds display  (1.5 days)

**Objective** Feeds are fetched and displayed properly in their components

- [ ] setup the `FeedIndex` component
  - [ ] pass on each feed to `FeedIndexItem`
- [ ] setup `FeedIndexItem` component
  - [ ] displays title and logo of website (are links to the website)
  - [ ] displays description of website (clicking opens up modal with detail)
  - [ ] displays an "Add" button (clicking opens up a different sidebar with adding collection)
  - [ ] displays the photo and title of the first article (clicking opens an ArticleDetail)
- [ ] test by placing `FeedIndex` in DOM

### Phase 3.5: FeedIndex and FeedIndexItem, deploy to Heroku (0.5 days)

- [ ] style `FeedIndex` to hold `FeedItem`s with proper spacing
- [ ] make `FeedIndexItem` resemble the ones on Feedly website
- [ ] deploy to Heroku

### Phase 4: Collections Model, API, basic APIUtil, and Store  (1 day)

**Objective:** Collections can be created, read, edited, and destroyed through the API

- [ ] create `Collection` model
- [ ] CRUD API for collections, should be nested under single user (`CollectionsController`) (Under 'Organize' in sidebar)
- [ ] jBuilder views for collections
- [ ] seed the database with some collections under existing users
  - [ ] Add feeds to collections
- [ ] test APIUtil interaction with API in the console
- [ ] implement `CollectionClientActions` and `CollectionServerActions` methods for collections
- [ ] create `CollectionStore`
- [ ] test action and store methods

### Phase 5: Sidebar (1 day)

**Objective** Display a sidebar with the username, collections and their feeds, and other links when logged in, else generic page

- [ ] Make a sidebar component
  - [ ] two cases: logged in or not logged in
  - [ ] displays different things depending on log in state
- [ ] logged in display  
  - [ ] username at the bottom, with logout button
  - [ ] has a "pin" button
    - [ ] add functionality to make the side bar keep displayed
    - [ ] change text of "pin" to "unpin" and vice versa  
  - [ ] has a Today link
  - [ ] has a save for later link
  - [ ] has a link to an add content
  - [ ] user's collections are shown (clicks show the collection)
    - [ ] each collection has a dropdown that displays the feeds
  - [ ] has a "organize collections" link
- [ ] logged out display  
  - [ ] has title of website and brief catch phase
  - [ ] has login button
  - [ ] has login as demo user (with a short descriptive text)
  - [ ] has sign up button
  - [ ] buttons open up a modal with form
- [ ] Add the styles to make it look nice

### Bonus (TBD)

- [ ] FeedIndexItem has number of readers, number of articles/Week
- [ ] FeedIndexItem photo is black and white initially, then fades into color
- [ ] Modals can have multiple tabs
- [ ] Preferences link
