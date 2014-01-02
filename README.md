JUST EAT Developer Recruitment Test
==================================

Thank you for taking the time to do our technical test. It consists of two parts:

* A coding test
* A few technical questions

# Coding Test

JUST EAT has a public API available at http://api-interview.just-eat.com/ that you can use to get restaurant information, including which restaurants deliver to what areas.

As an example, http://api-interview.just-eat.com/restaurants?q=se19 returns a list of restaurants that deliver to an outcode, including some basic restaurant information (for outcode = se19).

The API requires you specify a set of valid request headers before it'll respond.

		Accept-Tenant: uk
		Accept-Language: en-GB
		Accept-Charset: utf-8
		Authorization: Basic VGVjaFRlc3RBUEk6dXNlcjI=
		Host: api.just-eat.com

The task is to create a command line application using C# and Visual Studio 2012 that accepts a postcode as a parameter. The application should then display the following information about each restaurant that delivers to that postcode.

* Name
* Rating
* Types of food for the restaurant

The restaurants should be ordered from highest rating to lowest rating.

- We use [NUnit](http://www.nunit.org) and [Moq](http://code.google.com/p/moq) in a lot of our software, references have been added using [NuGet](http://nuget.codeplex.com/) Packages. Everything is in place for you to just write the code (no "File > New Project" required).
- We've enabled [NuGet] package restore, so don't worry about sending us compiled binaries.

## Task requirements

- All stories to be completed with an appropriate level of testing.
- Feel free to use whatever testing, mocking or stubbing frameworks you prefer, along with any other packages you like.
- Your code should be of production quality.
- Clone our git repository locally and work on your solution
- In order to avoid bounced emails we would like you to submit your results by uploading the relevant zip file to a shared Google Drive folder. Please send an email to tech.recruitment@just-eat.com with your **valid Google email address** so we can give you the correct upload permissions.

## User stories

### Story 1 - Accepting command line input

As a **user running the command line application**<br />
I can **supply a valid outcode on the command line**<br />
So that **I can query the JUST EAT API for results**

#### Acceptance criteria

* Command line parameter accepted

---

### Story 2 - Querying the API

As an **API consumer**<br />
I want to **query the restaurant API**<br />
So that **I can output core restaurant details**

#### Acceptance criteria

* Must provide valid headers
* For known outcode se19, some results are returned

---

### Story 3 - Outputting results

As a **user running the command line application**<br />
When I **search for a valid outcode**<br />
I want **restaurant details printed into console window**

#### Acceptance criteria

* Name, rating and types of food for the restaurant printed into console window

---

### Story 4 - Sorting results

As a **user running the command line application**<br />
When I **output core restaurant details**<br />
I want **to see restaurants ordered correctly**

#### Acceptance criteria

* Restaurants ordered and outputted on screen
* Restaurants ordered highest to lowest

# Technical questions

Please answer the following questions in a markdown file called `Answers to technical questions.md`.

* Did you have time to complete the coding test? What would you add to your solution if you had more time?
* What was the most useful feature in your opinion that was added to C# 4? Please include a snippet of code that shows how you've used it.
* What's your favourite programming language? Why?
* How would you track down a performance bottleneck in a .NET application? Have you ever had to do this?
* How would you improve the Just Eat public API found here?: http://www.just-eat.co.uk/webservice/webservices.asmx
* Please describe yourself using either XML or JSON.


Thanks for your time, we look forward to hearing from you!
- The [Just-Eat dev team](http://github.com/justeat)
