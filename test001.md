1.What is the proposed name for your Web application?
The name for my web application is Neverland, because users could share something they really love and put great enthusiasm with other users. It is a platform where users show their true selves. 
  
2. Who is the target audience?
target audience: The people who have passions for personal interests, creating and sharing life with others. So fashionable young people, artists, and the group of people sensitive to visual experience are the target audience. 

3. What problem is it intended to solve for the target audience?
The web application is a microblogging platform, a little like Tumblr. 
a) It can provide some kind of social functions. People having particularly interest in something are always eager to find others of the same hobby. This application provides opportunities for them. By posting pictures and tagging, other users can find them easily and communicate through instant messages. Photographers, designers, writers and musicians may benefit a lot from this application.
b) This is a platform where every body could show their works and talents to the world. The sense of accomplishments users gain when they receive like from others will encourage them to keep the passion and continuously move forward.  
c) The application is also a good choice for people to record their lives. The operation is simple and convenient, which could satisfy users’ requirements in the fragmented and efficient world.

4. How will it meet the minimum project requirements?

5. Why is your proposed Web application unique or creative beyond simply meeting the minimum requirements?

# TODO : Your Project Name

TODO : Please provide a detailed project description.

## Build status

TODO : Modify to match your project specific Travis Build
[![Build Status](https://travis-ci.org/infsci2560sp17/full-stack-web.svg?branch=master)](https://travis-ci.org/infsci2560sp17/full-stack-web-wenxxx)

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