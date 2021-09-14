---
title: "CS Summer Checklist"
date: 2021-09-12T10:37:19-04:00
draft: false
---

## Goals

1. Establish your reputation by showing employers your *Proof Of Skill*
2. Setup a personal website to showcase your projects 
3. Introduction to technical interviews
4. Have fun — life is short
    - Seriously, it’s all going to work out.

## Proof Of Skill
- [ ]  Build an application that solves a small problem
- [ ]  Show it to the world by deploying it with Heroku, GitHub Pages, Netlify, or AWS/GCP (in order of easiest to hardest)

The point of this is for you yourself to learn how to go from an idea in your head to a tangible product that anyone in the world can use (AKA the process of software engineering). Once you can do it yourself and employers can see that you've done it yourself, you'll stand out amongst the crowd. It will be a no-brainer for them to take a chance on you with an interview. As a bonus, it will give you something substantial to talk about in your interviews as well. 

In college, I got away with showcasing [projects](https://github.com/visaals/Portfolio) from college classes and [stuff](https://github.com/cameronjump/puzzlr) I built with friends at hackathons. Hackathons are great because you don't have to scramble to find time between exams and class projects. Since y’all started CS way before me, this is a chance to get 1 step ahead. 

Here’s an example app, [Pinpoint Neighborhoods](http://pure-wave-86480.herokuapp.com/), that I made for fun, built on React, using the [Google Maps API](https://developers.google.com/maps) and [OpenRouteService API](https://openrouteservice.org/dev/#/api-docs). It will find the best neighborhood for you to live in based on what locations you want to live near. 


![pinpoint neighborhoods](pinpoint_neighborhoods_2.png)
*If I want to live near a Trader Joe's and Blue Bottle Coffee shop in NY, it tells me I should live in Midtown East, Manhattan*


Seem complicated? Maybe at first. However, once you understand that all applications online are made up of 3 basic components, what I did will seem trivial. All I did was build out a Frontend UI and string together some already existing Backend APIs (on their free tiers). If I wanted to add managing user accounts, I will eventually have to connect my app to a Data Layer.

Soon, you'll be able to bring your ideas to life too, all by typing a bunch of keys on your keyboard, just like I figured out how to anser the question "what's the best neighborhood to live in if I want to be within 10 minutes of coffee, groceries, etc." to build Pinpoint Neighborhoods.

Let's get started! Most applications are made of these 3 core components:

### Frontend UI

Choose Web or Mobile. Examples include React, Swift, Android, React Native, etc. 

- [ ]  Build an interactive UI that takes in some input data with a basic form, calls an API, and displays output to the user

Along the way, you might end up learning:

- The basics of the Model-View-Controller architecture
- UI state management is hard, but frameworks like React try to make them easier
- Making things look nice is also hard —> check out Bootstrap
- In JavaScript “callback hell” and you’re forced to figure out how to code asynchronously

### Backend API

- [ ]  Build a basic HTTP server

Every language should come with a library to setup a basic HTTP server. If you’re just starting out, I’d suggest building an API in JavaScript (Node/Express), Python, or Go.

- [ ]  Call your HTTP server from the Frontend UI

Run the server in the command line and attempt to call the API from the Frontend UI to return some useful information.

- [ ]  Retrieve information from a free online API

Find a free API online and call it from your backend HTTP Server API. For instance, your backend API could call a free Weather API to get today’s forecast, a Crypto Exchange API to get the price of bitcoin, the Google Maps API to get restaurants near you, use IMDb’s API to analyze movies, etc. 

Along the way, you’ll learn:

- Basics of RESTful interfaces (GET, PUT, POST, etc.)
- Running servers at a host/port and calling it from your frontend, glueing together your frontend and backend
- How to parse JSON
- Basic API authentication using tokens
- How to deploy your API to the world and use it from anywhere with an internet connection

### Data Layer

Use a database to store data for your application. For example, you could use Firebase, MySQL, MongoDB, etc. 

Along the way, you’ll learn:

- How to setup a database and connect to it from your Frontend UI or Backend API using a connection string
- The basics of MySQL
- How to setup tables with fields and figuring out what is the primary key, what concepts you should separate out into different tables, etc. For example, if you’re storing user information for a social media app, you might make a User table, Posts table, etc. How would you model a friend request? How would you retrieve all the posts for a given user? How would you retrieve all the posts from a User’s friends to build a newsfeed?

## Personal Website

Throughout your career, it’s to your benefit if you establish a personal brand of who you are, what you’ve built, and what skills you bring to the table. It’s a career-long process that compounds over time, and we’re just going to lay the foundation. Your personal website should be an extended, more interesting version of your resume. 

Start with using GitHub Pages, a free hosting service that let’s you put a static website at `<github-username>.github.io`

- [ ]  Create a page on GitHub Pages and summarize your project with a description of what it is, how you built it, what you learned, and plenty of screen shots or GIFs
- [ ]  Create an `About` , `Projects` , and `Writing` page

e.g. [https://visaals.github.io](https://visaals.github.io) is what I used to showcase my projects in college

Create an `About` page and a `Projects` page. Over time, you’ll add projects to showcase new things you’ve learned. You can also write blog posts or tutorials to help others on their career journey. The best person to learn from is someone just a couple steps ahead of you because they remember the struggles you’re dealing with now.  Software Engineering is a positive sum game. You win by helping others win. 

I need to add more posts (especially technical ones) to `https://visaalambalam.com`

Here's an example of some top 1% personal websites

- [https://intuitiveexplanations.com/](https://intuitiveexplanations.com/)
- [https://jeremyaguilon.me/blog/ranking_interview_questions_by_cram_score](https://jeremyaguilon.me/blog/ranking_interview_questions_by_cram_score)

By no means does your website have to be as detailed as the examples above to do well, but it can only help you and others.

## Technical Interviews

It’s a bit early to start preparing for these during your freshman year summer, but if you’re curious and are satisfied with your project, take a look at [leetcode.com](http://leetcode.com) and do the “most liked, easy” problems to start with.

Here are the most important categories to understand deeply: 

- [ ]  HashTable
- [ ]  Array
- [ ]  String
- [ ]  Graph (BFS, DFS)
- [ ]  Trees (Binary Tree Traversal)
- [ ]  Sorting (MergeSort)
- [ ]  Searching (Binary Search, Graph Searches)

Start with “Reverse a String”, “Reverse a Linked List”, “2Sum”  problems. If you’re feeling adventurous, attempt the “Word Search” problem.

Focus on understanding how *and why* these core data structures and algorithms work. If I asked you to explain how a hash table works under the hood, could you explain it by heart AND answer follow up questions? Why would you pick a BFS over a DFS? ALWAYS think about tradeoffs with each decision you make. Should I use an Array or List? Should I represent my graph as a 2D array or an Adjacency List? Evaluating tradeoffs are the bread and butter of engineering and interviewing. 

In the future, how you solve these problems is just as important as getting the right answer in a 45-60 minute interview. More to come next year!

## Most importantly, have fun.

Pick a project that compels you. Try to find DS/Algorithms that you find cool and don’t put too much pressure on yourself if you make mistakes. Follow your curiosity. If you wondered how auto-complete works, there’s a leetcode question for that! It’s pretty cool and uses a Trie data structure. 

Luckily for you, CS is not a zero sum game like applying to medical schools. There is an abundance of jobs. If you don’t get the best internship the first year, there’s always the next year. The same applies to after you graduate. You have time and there’s no pressure. Enjoy the journey because if you don’t, pick a different career. 

- [ ]  Have fun (required)

