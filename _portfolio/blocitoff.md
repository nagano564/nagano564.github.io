---
layout: post
title: Kenny's Chat
thumbnail-path: "img/bloc-chat.png"
short-description: Kenny's Chat uses Firebase and AngularJS to create a real-time chat application.

---

{:.center}
![]({{ site.baseurl }}/img/bloc-chat.png)

## Explanation

Bloc chat was my next project where I had two major tasks
1) functions as a basic chat web app
2) integrates a database for real-time messaging.
To make it all work, I built Bloc Chat with the AngularJS framework and connected it to Firebase.

## Problem

The most important thing to know about Bloc Chat is that, unlike Bloc Jams, where I was given lots of instructions and explanations by the Bloc curriculum, the Bloc Chat project was essentially, “Here’s what should happen. Figure it out.”

## Solution

Google and the aforementioned documentation is what I depended on, and for once, I felt like I was using crossover skills like proper research, reading between the lines, reading ALL THE LINES, understanding what applies and what doesn’t.
As frustrating as not getting a certain feature to work is, the light bulb going off after figuring it out is the most
satisfying parts of being a web developer. It's a profession where I am never going to know everything and always having to learning
is part of programming that I love.

## Working With Firebase

For me, the most challenging part of Bloc Chat was working with the Firebase database. This was my first time creating a database from scratch, manually connecting it to a web app, and then writing the code that automatically sends information to the database and displays that information in the browser. I didn’t know it at the time, but I was building a relational database structure (mind you, a very, very simple version). Essentially, the database holds two object types, and they are related like this:

```
bloc-chat
|—> rooms
|    |—> -KjM2Ktq-eXy4wCnGP: “kenny”
|—> messages
|    |—> -KjtyDv82UyqJGkvcO
|        |—> content: “this is a message in the kenny chat room”
|        |—> roomId: “-KjM2Ktq-eXy4wCnGP”
|        |—> sentAt: “time date”
|        |—> username: “testing123”
```
As you can see, there’s an overarching bloc-chat object, and it holds the rooms and the messages. Each room is identified by a unique key (in this case, that’s the -KjM2Ktq-eXy4wCnGP). Each message is also identified by a unique key of its own, but stored under that key is the roomId key, which holds as its value the key to the room which the messages belongs.

Being a beginner, I had expected the messages to actually fall under the rooms where they belonged rather than be separated and only connected by a number. However, after seeing it in action, and after reading through all of the Firebase documentation on best practices to structure data, it makes perfect sense now. Had I followed through on what I originally expected to happen, I would have committed the first data structure error listed in the documentation, resulting in the browser having to download more information than is necessary upon simply opening Bloc Chat, which would make for a rather slow and bandwidth-expensive experience.
