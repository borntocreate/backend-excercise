# Backend Excercise

You will create a basic JSON API using PHP and SQL.

1. Implement a login/logout to authorize for the API:
    - Implement a route `/auth/login` which grants the client API access
    - Mandatory fields are `username` and `password`
    - Implement a route `/auth/logout` which revokes the clients API access

1. Implement a route accepting a `POST` request to `/auth/login` which accepts a `username` and `password` as input and authorizes the user for the API when credentials are valid.



2. Implement the following models:
    1. Post
        - id
        - title
        - author
        - content
        - dateCreated
        - dateUpdated
    2. Author
        - id
        - firstName
        - lastName
        - dateCreated
        - dateUpdated
  
3. Implement a persistence layer for `Post` and `Author`
  
3. Implement `GET` route for `/posts` which returns all posts
    - Implement a pagination
    - Implement a search by `title`, `content` and `author`
    - Implement optional order parameters
  
4. Implement a `POST` route for `/posts` which registers a new post
    - Mandatory fields are `title`, `author`, `content`
    - Content can contain `HTML`
  
5. Implement `GET` route for `/author` which returns all `Authors`
    - Implement a pagination
    - Implement a search by `firstName` and `lastName`
    - Implement optional order parameters
  
6. Implement a `POST` route for `/author` which registers a new `Author`
    - Mandatory fields are `firstName` and `lastName`
    
Implement all changes following PHP best practices ([PSR-1](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-1-basic-coding-standard.md), [PSR-2](https://www.php-fig.org/psr/psr-2/)) and [basic security principles](https://www.owasp.org/index.php/Security_by_Design_Principles).
