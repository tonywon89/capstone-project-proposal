## Component Hierarchy

* `App`
  * `Sidebar`
    * `SidebarCollectionIndex`
    * `SidebarCollectionIndexItem`
  * `Children`
    * `Home` (Index Route)
      * `CollectionDetail` (for `Today` collection)
        * `ArticleIndex`
          * `ArticleIndexItem`
    * `CollectionIndex`
      * `CollectionIndexItem`
        * `FeedItem`
    * `FeedIndex`
      * `FeedIndexItem`
        * `FeedIndexItemArticle`
    * `CollectionDetail`
      * `ArticleIndex`
        * `ArticleIndexItem`
  * `Details`
    * `FeedDetail`
    * `ArticleDetail`
  * `AddFeedSidebar`
    * `AddFeedCollectionIndex`
      * `AddFeedCollectionIndexItem`
