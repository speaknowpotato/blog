# REST, RPC


REST (REpresentational State Transfer) is a software architectural __style__. It's a style. 

You can understand it like - we have HTTP, and engineers found out a code structure style that works very well for backend-frontend communication via HTTP.


gRPC grpc.io/ (opens new window)is an open-source framework (Originally developed by Google). It is a framework. So you use it just like other frameworks/libraries - you install it by cloning the GitHub repo, or from a package manager (e.g. Web runtime library is npm i grpc-web). It supports all the common backend/frontend languages.

## REST

### Pros and Cons
Pros

1. Just HTTP calls. HTTP is the backbone of the web, so any platform / language come with it. You use it almost anywhere - within your app, inside browser devtool, or just curl.
2. Easy to build. As you can see above, it's just a few lines of code to build and use REST API. (But building a good one definitely requires more work)

Cons

Need the backend and the frontend in sync. As you can see, there's no contract between the backend and the frontend. The frontend has to know the path, method, request format, etc. And whenever the backend changes, the frontend also needs to keep changes in sync manually.
Easy to write messy APIs. You have the total control of what you do, so you can have APIs with inconsistent naming, behavior. E.g. Nothing prevents you from making GET /list delete all the items.




## GRPC

High-performance, minimal payload


In gRPC, the structure is defined in the code, and only data is transferred. 


### Implementation
Once you have the proto definition, you load the proto file into your backend to implement the API features. And you run a command to generate the client-side code and use that in the frontend code.


## Reference
[https://liyangguang.com/blog/2020/05/rest-grpc-graphql/
](https://liyangguang.com/blog/2020/05/rest-grpc-graphql/
)