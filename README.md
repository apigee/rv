![RV](/images/rv.png?raw=true)

# RV


Web API design guidelines for crafting interfaces that developers love.


## Contact Us

Your input is appreciated. Feel free to file a GitHub Issue, a Pull Request, or contact us. Thank you!

- [@ResourceVerb](https://twitter.com/resourceverb)
- <mailto:rv@apigee.com>


## Example

## Introduction

## Philosophy

RV 

A pattern language for APIs. 

* The biggest problem all APIs face is adoption.
  * This is a people problem. Do things that make it easier and faster for people to use your services. (reference value)
* Things, entities, must be addressable
  * URLs are addresses for things
* People need to understand the high level organization of the system
  * Collections/entities
* Things must be created and destroyed (and updated and retrieved)
  * Use HTTP verbs. They are the basic palette with which you paint (CMYK)
* Things that move must have their address updated. Note: moving is precarious and should only be done when truly necessary.
* When the structure of a representation changes, clients will break.
  * Give clients solid ground and don't shift it on them. This is the beginning of versioning.
* When you have to shift the ground on people (change the structure of a representation), provide time for migration.
* When there are errors, people will need to understand how to fix them.
  * Provide error information for people (not just machines).
* APIs are built for clients. Without developing a client in parallel, you are imagining the requirements. Design in perspective. Orthographic drawings tell you everything you need to know to construct a building, but they won’t tell you how it feels to be in it.
* No design system is or should be perfect. 
  * Nonconforming oddities can be enriching. (could be stricken, but something along these lines feels appropriate)
* You will have to control access to your API.
  * Use OAuth. But that is a big hammer, so allow basic auth and API keys.
* Bad actors can hurt the performance of your system.
  * Implement spike arrests and rate limiting.
* You will need to understand how the system is being used. 
  * Analytics. (whole set of patterns here)
* It is not possible to understand how people will use an API that hasn't been released.
  * Ship something. No matter how much time you spend thinking about design, there is no substitute for feedback from real usage. Be pragmatic.
  * Don't be clever
* Never, ever, ever, ever, ever push complexity onto developers. Example: response for an endpoint that can give multiple entities but doesn't wrap a singleton in an array.

## Guidelines

### Collections

### Entities

### Versions

### Query Parameters

### Header Parameters

### Conveniences

### Formats

### Actions

### Authentication

### Dates

### Filters

### Pagination

### Hypermedia

### Errors

### SDKs