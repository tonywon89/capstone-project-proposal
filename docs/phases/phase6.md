# Phase 6: Flux Architecture for Collections and Articles and React Router

## Rails
### Models

### Controllers

### Views

## Flux
### Views (React Components)
* CollectionsIndex
 - CollectionIndexItem
 - CollectionFeedItem
* CollectionArticles
* CollectionFeedDetail

* ArticleDateIndex
* ArticleItem

### Stores
* ArticleStore

### Actions
* CollectionActions.fetchCollections
* CollectionActions.createCollection
* CollectionActions.fetchSingleCollection
* CollectionActions.updateCollection
* CollectionActions.destroyCollection

* ArticleActions.receiveArticle
* ArticleActions.removeArticle

* ApiActions.notifySave -> for articles
* ApiActions.removeCollectionArticle

### ApiUtil

* ApiUtil.saveArticle
* ApiUtil.unsaveArticle
* ApiUtil.associateArticle

## Gems/Libraries
