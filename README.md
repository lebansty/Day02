# Day02
Write a blog on Difference between HTTP1.1 vs HTTP2
Ans:
 HTTP1.1
 It was introduced in 1997.Features like CORS, keep-alive was introduced in this update.
 For every TCP connection there could be multiple requests and responses, and pipelining where the client can request several resources from the server at once. However, pipelining was hard to implement due to issues such as head-of-line blocking and was not a feasible solution.
A warning header field to carry additional information about the status of a message was introduced. Can define 24 status codes, error reporting is quicker and more efficient.
It is relatively secure since it uses digest authentication, NTLM authentication.
Expands on the caching support by using additional headers like cache-control, conditional headers like If-Match and by using entity tags.
HTTP/1.1 provides faster delivery of web pages and reduces web traffic. However, TCP starts slowly and with domain sharding (resources can be downloaded simultaneously by using multiple domains), connection reuse and pipelining, there is an increased risk of network congestion.

HTTP 2
It was introduced in 2015.
Uses multiplexing, where over a single TCP connection resources to be delivered are interleaved and arrive at the client almost at the same time. It is done using streams which can be prioritized, can have dependencies and individual flow control.
It provides a feature called server push that allows the server to send data that the client will need but has not yet requested.
Underlying semantics of HTTP such as headers, status codes remains the same.
Security concerns from previous versions will continue to be seen in HTTP/2. However, it is better equipped to deal with them due to new TLS features like connection error of type Inadequate_Security.
HTTP/2 does not change much in terms of caching. With the server push feature if the client finds the resources are already present in the cache, it can cancel the pushed stream.
HTTP/2 utilizes multiplexing and server push to effectively reduce the page load time by a greater margin along with being less sensitive to network delays.

Write a blog about objects and its internal representation in Javascript.
Objects, in JavaScript, is it’s most important data-type and forms the building blocks for modern JavaScript. These objects are quite different from JavaScript’s primitive data-types in the sense that while these primitive data-types all store a single value each.
Objects are more complex and each object may contain any combination of these primitive data-types as well as reference data-types.
An object, is a reference data type. Variables that are assigned a reference value are given a reference or a pointer to that value. That reference or pointer points to the location in memory where the object is stored. The variables don’t actually store the value.
Objects are more complex and each object may contain any combination of these primitive data-types as well as reference data-types.
An object, is a reference data type. Variables that are assigned a reference value are given a reference or a pointer to that value. 
That reference or pointer points to the location in memory where the object is stored. The variables don’t actually store the value.
