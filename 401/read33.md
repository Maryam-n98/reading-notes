# Read 33 : API (GRAPHQL)

* Serverless: it is a cloud computing execution model that could manage the distribution and the providing of severs.
* Using cloud providers in serverless make a lot of money
![img](https://camo.githubusercontent.com/b96a4953d27e027cb980c00d02daa1b9ae0f98173ff3ca1b001f07d5f502d312/68747470733a2f2f6861636b65726e6f6f6e2e636f6d2f686e2d696d616765732f312a74344f34555870644736384d51626f4e4b43366242772e6a706567)

### Traditional vs. Serverless Architecture
![img](https://camo.githubusercontent.com/07ba0f519f9fda2d8fa89b383dcaae5188c6889394a1d1f62723816edd80abab/68747470733a2f2f6861636b65726e6f6f6e2e636f6d2f686e2d696d616765732f312a785f76354e52433354544d74314d61596c31674d55672e6a706567)

* The benefits of using serverless:
  * It is reduce cost
  * Setting up environments are easy

* The disadvantages of using serverless:
  * you cannot directly access APIs through the usual IP, because serverless functions are accessed only as private APIs. 
  * unusable for applications that have variable execution times
  

* If your context's of project is simple use serverless, else use traditional architecture.
* Faas is an implementing for serverless that can use to deploy individual functions or a piece of business logic.

* Principles of FaaS:
  * Complete management of servers
  * Invocation based billing
  * Event-driven and instantaneously scalable

* With Serverless, everything is stateless

The serverless app
![img](https://camo.githubusercontent.com/c2dc0f9346cf51df7f2bca85159f7a8b439b2e739ddccabad6c2ceeaa8e3e914/68747470733a2f2f6861636b65726e6f6f6e2e636f6d2f686e2d696d616765732f312a5449726a4e37456a4c55564a6d4a36597648523744672e706e67)


## AWS Amplify
* AWS Amplify is a set of tools and services that can be used to build a scalable full-stack apps.
### AWS Amplify Advantages
  * the project can be connected to backend easily.
  * deploy static web apps in a few clicks
  * easily manage app content outside the AWS console

## Add relationships between types
* To define relationship between models, we have to use @connection
* many-to-many relationship can be defined using two one-to-many relations, an @key, and a joining @model.
* fields argument is used to queried by to get connected objects.
* A Has One @connection can only reference the primary index of a model
* Set the limit argument to define the number of nested objects, which is by default 100.
