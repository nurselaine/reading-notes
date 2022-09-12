## Class 08 Reading Notes: APIs

#### API Design Best Practices

1. What does REST stand for? 
  - Representational state transfer (REST) archetectural approach to web services 
2. REST APIs are designed around a ____.
3. What is an identifier of a resource? Give an example.
4. What are the most common HTTP verbs?
5. What should the URIs be based on?
6. Give an example of a good URI.
7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
8. What status code does a successful GET request return?
9. What status code does an unsuccessful GET request return?
10. What status code does a successful POST request return?
11. What status code does a successful DELETE request return?
###### Bookmark and Review
#### RegExr - Pay particular attention to the cheatsheet
#### Regex Tutorial
#### Regex 101

#### What I want to learn more about
- 

**GET** retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.
**POST** creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.
**PUT** either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.
**PATCH** performs a partial update of a resource. The request body specifies the set of changes to apply to the resource.
**DELETE** removes the resource at the specified URI.