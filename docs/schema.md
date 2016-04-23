#Schema Information

## users
column name     | data type | details
----------------|-----------|-----------------------
id              | integer   | not null, primary key
email           | string    | not null, indexed, unique
password_digest | string    | not null
session_token   | string    | not null, indexed, unique

Associations:  
  has_many: collections  
  has_many: feeds, through: collections  


##feeds

column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
name        | string    | not null
url         | string    | not null

**Will have a #parse that gets the information from the feed url**

Associations:

  has_many: collections, through: collection_feeds

  has_many: users, through: collections

##collection_feeds

column name   | data type | details
--------------|-----------|-----------------------
id            | integer   | not null, primary key
feed_id       | integer   | not null, indexed
collection_id | integer   | not null, indexed

Associations:  
    belongs_to: feed  
    belongs_to: collection  

## collections

column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
name        | string    | not null
user_id     | integer   | not null, indexed

Associations:  
  belongs_to: user  
  has_many: feeds, through: collection_feeds  
