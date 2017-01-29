1. What is the proposed name for your Web application?
---
My web application is called “Travel Pal in USA”. People can find travel pals in this platform.
  
2. Who is the target audience?
---
According to the name, this application aims at English-speaking people who want to travel in USA, and need to find one or more partners to travel together. 

3. What problem is it intended to solve for the target audience?
---
a)	Some people desire to travel to some places that no friends are interested in, however, they do not want to be alone. Some people have several travel partners but wants more for many reasons, like reducing average traveling fee and sharing rooms.
b)	It is often difficult for people to find proper travel partners in their social networks. On the one hand, their social networks are limited. On the other hand, they need to post their advertisements in many different places, such as Twitter, Facebook, and Weibo.  “Travel Pal in USA” provides the platform for them to easily find as many as possible people with the same travel desire. 

4. How will it meet the minimum project requirements?
---
a)	New users need to sign up if they want to interact with other users. Old users can sign in to their accounts.
b)	Users can search possible travel partners by filtering destination, departure, departure date, returning date, language, gender, and age.
c)	Registered users can see the travel plan of other users, and chat with other uses.

5. Why is your proposed Web application unique or creative beyond simply meeting the minimum requirements?
---
The interface is intuitive and easy to use, which help users find favorable travel partners conveniently and efficiently.




# TODO : Your Project Name
“Travel Pal in USA”

TODO : Please provide a detailed project description.

## Build status

TODO : Modify to match your project specific Travis Build
[![Build Status](https://travis-ci.org/infsci2560sp17/full-stack-web-wenxxx.svg?branch=master)](https://travis-ci.org/infsci2560sp17/full-stack-web-wenxxx)

## Web Site

TODO : Please provide a link to your web site ![](https://https://cryptic-sea-53580.herokuapp.com/)

## Key Features

TODO : Please list key features of your project.

* Key Feature 1
* Key Feature 2
* Key Feature N

## Project Details

### Landing Page

TODO : please provide a description of your landing page inluding a screen shot ![](https://.../image.JPG)

### User Input Form

TODO : please provide a description of at least 1 user input form including a screen shot ![](https://.../image.jpg)

## API

TODO : please provide a description of at least 1 API including a sample of request data and response data in both XML and JSON format.

### API Method 1

    POST photos/:id/tags

#### Parameters

- **id** _(required)_ — The Photo ID to add tags for.
- **tags** _(required)_ — Comma separated tags.

#### Response

A JSON or XMLobject containing the PhotoID and list of tags accepted.

#### Errors

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'error' keys describing the source of error.

- **404 Not Found** — The photo was not found.

#### Example

##### Request

    POST /v1/photos/123456/tags

##### Body

    tags=cute,puppy


##### JSON Response

```json
{
    "photoId": 123456,
    "tags": ["cute", "puppy"]
}
```

##### XML Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<PhotoTags>
    <photoId>123456</PhotoId>
        <tags>
            <tag>cute</tag>
            <tag>puppy</tag>
        </tags>
</PhotoTags>
```

## Technologies Used

TODO : List all technologies used in your project

- [Spring Boot](https://projects.spring.io/spring-boot/) - Takes an opinionated view of building production-ready Spring applications.
- [Thymleaf](http://www.thymeleaf.org/) - Thymeleaf is a modern server-side Java template engine for both web and standalone environments.
- [Maven](https://maven.apache.org/) - Apache Maven is a software project management and comprehension tool.