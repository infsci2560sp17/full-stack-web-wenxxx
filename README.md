## Travel Pal in USA

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


## Build status
[![Build Status](https://travis-ci.org/infsci2560sp17/full-stack-web-wenxxx.svg?branch=master)](https://travis-ci.org/infsci2560sp17/full-stack-web-wenxxx)

## Changelog

[Changelog](Changelog.md)

## Web Site

[](https://https://cryptic-sea-53580.herokuapp.com/)

## Key Features
* Registration: New users need to sign up if they want to interact with other users.
* Login: Old users can sign in to their accounts.
* Find a match: Users can search possible travel partners by filtering destination, departure place, language, and gender.
* Forum: Registered users can share or browser travel plan or experience, transportation method, and delicious food on the forum.


 ## Project Details

    ### Landing Page
    As for a welcome page, it includes title "Travel Pal in USA", the navigation bar with “homepage”, “find a match”, “forum”, "login", and "registration".
    In the middle of the page, the user will be welcomed by a cheerful American cartoon map.

    ### Home Page
    ![](https://github.com/infsci2560sp17/full-stack-web-wenxxx/blob/master/src/main/resources/public/images/Homepage.png)
    ### Registration
    ![](https://github.com/infsci2560sp17/full-stack-web-wenxxx/blob/master/src/main/resources/public/images/Register.png)
    ### Log in
    ![](https://github.com/infsci2560sp17/full-stack-web-wenxxx/blob/master/src/main/resources/public/images/Login.png)
    ### Find a match
    ![](https://github.com/infsci2560sp17/full-stack-web-wenxxx/blob/master/src/main/resources/public/images/Match.png)
    ### Forum
    ![](https://github.com/infsci2560sp17/full-stack-web-wenxxx/blob/master/src/main/resources/public/images/Forum.png)


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

- [Spring Boot](https://projects.spring.io/spring-boot/) - Takes an opinionated view of building production-ready Spring applications.
- [Thymleaf](http://www.thymeleaf.org/) - Thymeleaf is a modern server-side Java template engine for both web and standalone environments.
- [Maven](https://maven.apache.org/) - Apache Maven is a software project management and comprehension tool.