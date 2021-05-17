# Which HTTP Status Code to Use for Every CRUD App
>
## HTTP Status CodesPermalink

A status code is a number higher than 100 and smaller than 600 that is part of a HTTP response. The first digit defines the class of the status. A status code comes with a reason phrase. The code is for programmatic recognition the phrase is for humans to understand what happened.

Every status code has to follow these two rules, even custom ones (yes the status codes are extensible).

## Status ClassesPermalink

If we understand the class a status code is in, we can locate problems more quickly.

**100 - 199Permalink**

These are informational status codes; they usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. Like using a different protocol or telling the client that its request will fail before they start sending the body.

**200 - 299Permalink**

These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.

**300 - 399Permalink**
These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. This can have multiple reasons, be temporary or permanent, but the client has to issue a request to the new location.

**400 - 499Permalink**
These are the client error codes. They are all about invalid requests a client sent to a server. There are several causes to this, timeouts, wrong URI, missing authentication, etc. A client is sending incorrect input and should confirm the input parameters are correct before retrying the request.

**500 - 599Permalink**
These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server. These errors can be temporary or permanent. Usually it’s best for the client to retry the same request.

## CRUD (Create, Read, Update, Delete)Permalink

The CRUD model defines the most basic API actions for persistent storage. Create, read, update, and delete. They make up the lions-share of API endpoints. Let’s see which status codes meet their requirements.

## API ChangesPermalink

If our API lives long enough, sooner or later it will change its structure. It’s best practice to avoid breaking changes and the redirection class of status codes can help with this because some clients follow their Location header automatically.

Status Codes

* 307 Temporary Redirect - This is the right code if the resource could be available on a different URL in the future, but we want the current endpoint to control where the client is redirected to. This status code will let the client come back to the current URL for every request.

* 308 Permanent Redirect - This is the right code if the resource will now be available at a new URL and the client should directly access it via the new URL in the future. The current endpoint can’t control the clients’ behavior after the request and a subsequent redirect if the resource URL changes again have to be issued from the new URL.

## Wrong URLPermalink

When a client sends a URL, we don’t know. This can have multiple different reasons, so we have to check which of them applies here.

## No PermissionsPermalink

Often clients can’t access every resource on the backend, so we need a way to tell them about it.

Status Codes

* 401 Unauthorized - The client hasn’t authorized itself to the backend yet and the server may give it access after that has happened.

* 403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

* 404 Not Found - If 401 or 403 is the case, but the backend doesn’t want to tell the client that the resource exists for security reasons.

## Refrenceses

[moesif blog](https://www.moesif.com/blog/technical/api-designWhich-HTTP-Status-Code-To-Use-For-Every-CRUD-App)
