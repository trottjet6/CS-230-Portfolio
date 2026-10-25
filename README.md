# CS 230 Portfolio – The Gaming Room

## Software Design Document
The completed software design document for Draw It or Lose It is included in this repository.

## Reflection

**Briefly summarize The Gaming Room client and their software requirements. Who was the client? What type of software did they want you to design?**
The client is The Gaming Room. They currently have an Android only game called Draw It or Lose It and wanted it expanded into a web based application that can run on multiple platforms. The software needed to support one or more teams, multiple players per team, unique game and team names, and only one instance of the game service in memory at a time.

**What did you do particularly well in developing this documentation?**
I kept the document organized around the client’s actual requirements and updated it consistently across the three projects. The Evaluation and Recommendations sections clearly compare the platforms and give a specific recommendation instead of staying general.

**What about the process of working through a design document did you find helpful when developing the code?**
Writing the domain model first made the Java classes clearer. Once Entity, Game, Team, Player, and the GameService singleton were defined in the document, it was straightforward to implement the same structure in code and test uniqueness and the single instance rule.

**If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?**
I would expand the early design constraints section with more detail on how the web based requirement affects the client side. Adding a short note on responsive design and browser testing earlier would have made the later evaluation sections connect more tightly.

**How did you interpret the user’s needs and implement them into your software design? Why is it so important to consider the user’s needs when designing?**
The user’s main needs were unique names, support for multiple teams and players, and only one game service in memory. I implemented those with an Entity base class, iterator checks before adding names, and a singleton GameService. Considering user needs early prevents building features that do not match what the client actually wants and reduces rework later.

**How did you approach designing software? What techniques or strategies would you use in the future to analyze and design a similar software application?**
I started with the requirements, then mapped them to classes and relationships using the UML diagram. Next I applied design patterns (singleton and iterator) to meet the constraints. In the future I would continue to separate the domain model from the platform specific pieces and document storage and memory decisions earlier so the architecture section is easier to justify.
