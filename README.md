#FeedMeScience

## Minimum Viable Product

FeedMeScience is a web application inspired by Feedly that will be built using Ruby on Rails and React.js. By the end of Week 9, this app will, at a minimum, satisfy the following criteria:

- [ ] New account creation, login, and guest/demo login
- [ ] Smooth, bug-free navigation
- [ ] Adequate seed data to demonstrate the site's features
- [ ] The minimally necessary features for a Feedly-inspired site: creating collections, adding or removing feeds to collections, displaying the feeds of the user, and providing feeds for the user to choose from
- [ ] Hosting on Heroku
- [ ] CSS styling that is satisfactorily visually appealing
- [ ] A production README, replacing this README

## Product Goals and Priorities

- [ ] Create an account (MVP)
- [ ] Log in/ Log out, including as a Guest/Demo User (MVP)
- [ ] Make collections (MVP)
- [ ] Display user's feeds and collections (MVP)
- [ ] Add and remove feeds from collections (MVP)
- [ ] Provide feeds for the user to choose from (MVP)
- [ ] Provides link to go to feed's website (MVP)
- [ ] Feeds display recent articles (MVP)
- [ ] Feeds show number of hits (expected feature, but not MVP)
- [ ] Categorizes feeds by date (expected feature, but not MVP)
- [ ] Mark article as read once user has clicked on article in feed (expected feature, but not MVP)
- [ ] Displays time the article was posted ( expected feature but not MVP)
- [ ] Able to organize collections (expected feature, but not MVP)
- [ ] Able to search for feeds (expected feature, but not MVP)
- [ ] Have subcategories of feeds (expected feature, but not MVP)
- [ ] Feeds have logos, Users have a profile picture (expected feature, but not MVP)
- [ ] Have a button to save articles to read for later (expected feature, but not MVP)
- [ ] User can hide or save articles (expected feature, but not MVP)
- [ ] User can choose how to display the articles of a feed (bonus feature)
- [ ] Embed videos for feeds with videos (bonus feature)
- [ ] Displays related feeds when displaying articles of a particular feed (bonus feature)
- [ ] User can mark all of the articles of a feed as read all at once (bonus feature)
- [ ] User can set preferences (bonus feature)
- [ ] User can select a theme for sidebar (bonus feature)
- [ ] User can share collections through a url (bonus feature)

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

### Phase 2

<!-- ### Phase 2: Collections Model, API, and basic APIUtil (1 day)

**Objective:** Collections can be created, read, edited, and destroyed through the API

- [ ] create `Collection` model
- [ ] seed the database with a small amount of test data
- [ ] CRUD API for collections, should be nested under single user (`CollectionsController`)
- [ ] jBuilder views for collections
- [ ] setup Webpack and Flux scaffold
- [ ] setup `APIUtil` to interact with the API
- [ ] test out API interaction in the console

### Phase 3: Flux Architecture and Router (2 days)

**Objective:** Collections can be created, read, edited, and destroyed with the user interfact.

- [ ] setup the flux loop with skeleton files
- [ ] setup React Router
- [ ] implement each collection component, building out the flux loop as needed -->
