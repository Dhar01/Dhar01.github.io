---
title: Web Fundamentals walk-through [TryHackMe]
published: true
---

# Task 2


A **DNS request** is made. When browser knows the server's IP address, it ask the server for the web page which is done with a **HTTP GET** request.

**GET** is an example of a HTTP verb, which are the different types of request. The server responds to the GET request with the web page content. IF the web page is loading extra resources, like *JavaScript*, *images*, or *CSS* files, those will be retrieved in <mark>separate GET requests.</mark>

For most websites now, these request will use **HTTPS**, a secure (*encrypted*) version of *HTTP*. This uses **TLS 1.3** (*normally*) encryption in order to communicate without:
- other parties being able to read the data.
- other parties being able to modify the data.

A **web server** is a software that receives and responds to HTTP(S) requests.
Example: **Apache**, **Nginx**, **Microsoft's IIS**.

HTTP runs on port 80 and HTTPS runs on port 443.

* What request verb is used to retrieve page content?

**Ans**: GET.

* What port do web servers normally listen on?

**Ans**: 80.

* What's responsible for making websites look fancy?

**Ans**: CSS.


# Task 3


#### Requests

There are 9 different HTTP "verbs", also known as methods. Each one has a different function.

**POST** requests are used to send data to a web server.

A HTTP request can be broken down into parts.
```http
GET /index.html
```

The next section is **headers**, which give the server more information about requests.

Finally, body of the requests. For POST requests, this is the content that's sent to the server.

#### Responses

The server reply with a response, a status. Normally it'll be a code. A basic breakdown of the status code is:
- **100-199** : information.
- **200-299** : Successes. (*200 OK is the "normal" response for a GET*)
- **300-399** : Redirects (*the information you want is elsewhere*)
- **400-499** : Client errors (*client did something wrong, like asking for something that doesn't exist*)
- **500-599** : server errors (*server tried, but something went wrong on their side*)


* What verb would be used for a login?

**Ans**:

* What verb would be used to see your bank balance once you're logged in?

**Ans**: GET.

* Does the body of a GET request matter? Yea/Nay

**Ans**: Nay.

* What's the status code for "I'm a teapot"?

**Ans**: 418.

* What status code will you get if you need to authenticate to access some content, and you're unauthenticated?

**Ans**: 401.


# Task 4



