# Read 08: Readings: APIs


### What does REST stand for?

REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.

### REST APIs are designed around a ____.

designed around resources.

### What is an identifer of a resource? Give an example.

A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

HTTP:
https://adventure-works.com/orders/1

### What are the most common HTTP verbs?

The most common operations are GET, POST, PUT, PATCH, and DELETE.

### What should the URIs be based on?

 resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

 ### Give an example of a good URI.

 https://adventure-works.com/orders // Good

 ### What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

  "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. Instead, you might want to denormalize the data and combine related information into bigger resources that can be retrieved with a single request. However, you need to balance this approach against the overhead of fetching data that the client doesn't need. Retrieving large objects can increase the latency of a request and incur additional bandwidth costs.
  bad

  ### What status code does a successful GET request return?

  GET request to the URI /add?operand1=99&operand2=1 would return a response message with the body containing the value 100. However, only use these forms of URIs sparingly.

###  What status code does an unsuccessful GET request return?

If the client sends a GET request to this endpoint, the response should contain the current status of the request. Optionally, it could also include an estimated time to completion or a link to cancel the operation.

### What status code does a successful POST request return?

A POST request creates a resource. The server assigns a URI for the new resource, and returns that URI to the client. In the REST model, you frequently apply POST requests to collections. The new resource is added to the collection. A POST request can also be used to submit data for processing to an existing resource, without any new resource being created.

### What status code does a successful DELETE request return?

The effect of a specific request should depend on whether the resource is a collection or an individual item. The following table summarizes the common conventions adopted by most RESTful implementations using the e-commerce example. Not all of these requests might be implemented—it depends on the specific scenario.

