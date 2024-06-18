* Use Resource Name (Noun) for the URL
* Use Plural
* 
* Use HTTP Methods the describe functionality

    |Method|Description|
    -------|-----------|
    |GET|Used to retrieve a representation of a resource.|
    |POST|Used to create new new resources and sub-resources|
    |PUT|Used to update existing resources|
    |PATCH|Used to update existing resources|
    |DELETE|Used to delete existing resources|

* Difference between Patch and Put ?


* Response Code
  * The client application behaved erroneously (client error - 4xx response code)
  * The API behaved erroneously (server error - 5xx response code)
  * The client and API worked (success - 2xx response code)
  * Reference:
    * https://www.restapitutorial.com/httpstatuscodes.html


* Provide example for the response

* Idempotent API design for POST to avoid repeated action
  * Bad: `POST /carts`
  * Good: `POST /carts (requestId: 12345)`

* Use Versioning
* Support Pagination
* Support Filtering
* Resource cross reference
  * Bad: `GET /carts/123?items=321`
  * Good: `GET /carts/123/items/321`
* Adding item
  * Bad: `POST /carts/123?addItems=321`
  * Good: `POST /carts/123/items {itemId: 12345}`
* Adding rate limit
* Reference
  * https://stackoverflow.blog/2020/03/02/best-practices-for-rest-api-design/