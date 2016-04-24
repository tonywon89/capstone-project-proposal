#CuriousFeed

## Minimum Viable Product

CuriousFeed is a web application inspired by Feedly that will be built using Ruby on Rails and React.js. By the end of Week 9, this app will, at a minimum, satisfy the following criteria:

- [ ] New account creation, login, and guest/demo login
- [ ] Smooth, bug-free navigation
- [ ] Adequate seed data to demonstrate the site's features
- [ ] The minimally necessary features for a Feedly-inspired site: creating collections, adding or removing feeds to collections, displaying the feeds of the user, and providing feeds for the user to choose from
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
- [ ] create `User` model
- [ ] authentication
- [ ] user signup/signin pages
- [ ] blank landing page after sign in

### Phase 2: Feeds Model, API, and basic APIUtil (0.5 day)

**Objective** Feeds can be retrieved through the API

- [ ] create `Feed` model
- [ ] seed the database with small amount of rss feeds from websites that provide it
- [ ] Retrieve feeds data by using an FeedAPI (`FeedsController`) to fetch the feed data
- [ ] jBuilder views for parsed data from Feed url using Feedjira gem
- [ ] setup Webpack and Flux scaffold
- [ ] setup  `ApiUtil` to interact with the API
- [ ] test out API interaction in the console
- [ ] setup `FeedStore`, `ServerActions`, `ClientActions`

### Phase 3: Frontend Feeds display  (1.5 day)

**Objective** Feeds are fetched and displayed properly in their components

- [ ] setup the `FeedIndex` component
  - [ ] setup spacing of between each `FeedIndexItem`
  - [ ] pass on each feed to `FeedIndexItem`
- [ ] setup `FeedIndexItem` component
  - [ ] displays title and logo of website (are links to the website)
  - [ ] displays description of website (clicking opens up modal with detail)
  - [ ] displays an "Add" button (clicking opens up a different sidebar with adding collection)
  - [ ] displays the photo and title of the first article (clicking opens an ArticleDetail)
- [ ] test by placing `FeedIndex` in DOM

### Phase 4: Collections Model, API and basic APIUtil (1 day)

**Objective:** Collections can be created, read, edited, and destroyed through the API

- [ ] create `Collection` model
- [ ] seed the database with a small amount of test data
- [ ] CRUD API for collections, should be nested under single user (`CollectionsController`)
- [ ] jBuilder views for collections
- [ ] setup Webpack and Flux scaffold
- [ ] setup `APIUtil` to interact with the API
- [ ] test out API interaction in the console

### Bonus (TBD)

- [ ] FeedIndexItem has number of readers, number of articles/Week
- [ ] FeedIndexItem photo is black and white initially, then fades into color
- [ ] Modals can have multiple tabs
- [ ]





<!-- ### Phase 2: Collections Model, API, and basic APIUtil (1 day)



### Phase 3: Flux Architecture and Router (2 days)

**Objective:** Collections can be created, read, edited, and destroyed with the user interfact.

- [ ] setup the flux loop with skeleton files
- [ ] setup React Router
- [ ] implement each collection component, building out the flux loop as needed -->
