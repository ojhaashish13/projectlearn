[LendingTree](../index.html)
============================

[V2Solutions](../index.html)

AFHTTPRequestOperation Class Reference {.hideInXcode}
======================================

-   Table of Contents
-   Jump To… Overview Tasks Properties     response     responseObject
        responseSerializer Instance Methods     -
    setCompletionBlockWithSuccess:failure:

-   [Overview](#overview)
-   [Tasks](#tasks)
    -   [Getting HTTP URL Connection
        Information](#task_Getting%20HTTP%20URL%20Connection%20Information)
    -   [Setting Completion Block Success / Failure
        Callbacks](#task_Setting%20Completion%20Block%20Success%20/%20Failure%20Callbacks)
-   [Properties](#properties)
    -   [response](#//api/name/response)
    -   [responseObject](#//api/name/responseObject)
    -   [responseSerializer](#//api/name/responseSerializer)
-   [Instance Methods](#instance_methods)
    -   [setCompletionBlockWithSuccess:failure:](#//api/name/setCompletionBlockWithSuccess:failure:)

-   [Index](../index.html)
-   [Hierarchy](../hierarchy.html)

AFHTTPRequestOperation Class Reference {.title .title-header}
======================================

  --------------- ------------------------------------------------------------------------------------
  Inherits from   [AFURLConnectionOperation](../Classes/AFURLConnectionOperation.html) : NSOperation
  Declared in     AFHTTPRequestOperation.h
  --------------- ------------------------------------------------------------------------------------

Overview {.subtitle .subtitle-overview}
--------

`AFHTTPRequestOperation` is a subclass of `AFURLConnectionOperation` for
requests using the HTTP or HTTPS protocols. It encapsulates the concept
of acceptable status codes and content types, which determine the
success or failure of a request.

Tasks {.subtitle .subtitle-tasks}
-----

### Getting HTTP URL Connection Information {.subsubtitle .task-title}

-   `  response` property
-   `  responseSerializer` property
-   `  responseObject` property

### Setting Completion Block Success / Failure Callbacks {.subsubtitle .task-title}

-   `– setCompletionBlockWithSuccess:failure:`

Properties {.subtitle .subtitle-methods}
----------

### response {.subsubtitle .method-title}

The last HTTP response received by the operation’s connection.

`@property (readonly, nonatomic, strong) NSHTTPURLResponse *response`

#### Declared In {.method-subtitle}

`AFHTTPRequestOperation.h`{.declared-in-ref}\

### responseObject {.subsubtitle .method-title}

An object constructed by the `responseSerializer` from the response and
response data. Returns `nil` unless the operation `isFinished`, has a
`response`, and has `responseData` with non-zero content length. If an
error occurs during serialization, `nil` will be returned, and the
`error` property will be populated with the serialization error.

`@property (readonly, nonatomic, strong) id responseObject`

#### Declared In {.method-subtitle}

`AFHTTPRequestOperation.h`{.declared-in-ref}\

### responseSerializer {.subsubtitle .method-title}

Responses sent from the server in data tasks created with
`dataTaskWithRequest:success:failure:` and run using the `GET` / `POST`
/ et al. convenience methods are automatically validated and serialized
by the response serializer. By default, this property is set to an
AFHTTPResponse serializer, which uses the raw data as its response
object. The serializer validates the status code to be in the `2XX`
range, denoting success. If the response serializer generates an error
in `-responseObjectForResponse:data:error:`, the `failure` callback of
the session task or request operation will be executed; otherwise, the
`success` callback will be executed.

`@property (nonatomic, strong) AFHTTPResponseSerializer<AFURLResponseSerialization> *responseSerializer`

#### Discussion {.method-subtitle}

**Warning:** `responseSerializer` must not be `nil`. Setting a response
serializer will clear out any cached value

#### Declared In {.method-subtitle}

`AFHTTPRequestOperation.h`{.declared-in-ref}\

Instance Methods {.subtitle .subtitle-methods}
----------------

### setCompletionBlockWithSuccess:failure: {.subsubtitle .method-title}

Sets the `completionBlock` property with a block that executes either
the specified success or failure block, depending on the state of the
request on completion. If `error` returns a value, which can be caused
by an unacceptable status code or content type, then `failure` is
executed. Otherwise, `success` is executed.

`- (void)setCompletionBlockWithSuccess:(void ( ^ ) ( AFHTTPRequestOperation *operation , id responseObject ))success failure:(void ( ^ ) ( AFHTTPRequestOperation *operation , NSError *error ))failure`

#### Parameters {.method-subtitle .parameter-title}

*success*
:   The block to be executed on the completion of a successful request.
    This block has no return value and takes two arguments: the receiver
    operation and the object constructed from the response data of the
    request.

*failure*
:   The block to be executed on the completion of an unsuccessful
    request. This block has no return value and takes two arguments: the
    receiver operation and the error that occurred during the request.

#### Discussion {.method-subtitle}

This method should be overridden in subclasses in order to specify the
response object passed into the success block.

#### Declared In {.method-subtitle}

`AFHTTPRequestOperation.h`{.declared-in-ref}\

-   [Index](../index.html)
-   [Hierarchy](../hierarchy.html)

* * * * *

© 2014 V2Solutions. All rights reserved. (Last updated: 2014-05-06)\
 Generated by [appledoc 2.2 (build
963)](http://appledoc.gentlebytes.com).
