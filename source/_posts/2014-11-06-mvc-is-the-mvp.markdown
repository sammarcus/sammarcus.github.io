---
layout: post
title: "MVC is the MVP"
date: 2014-11-06 14:52:51 -0500
comments: true
categories: Flatiron School
---

<p align="center"><img src="http://i.imgur.com/3LntWLt.gif" alt="Jake" /></p>

 We were originally introduced to the Model, View and Controller concept, or MVC, 2 weeks ago when we started SQL and Active Record. Knowledge often flies very fast here and it can be difficult to ascertain what we’ll definitely need to grasp and other ideas that we may be able to lookup and reference later. When MVC stuck around in Rails I knew it was something worth spending the time to get to know. When I knew I needed to tweak something but didn't know exactly where to do it, I would furiously toggle between all three and try to play a guessing game. Highly ineffective.

The idea of this three pronged approach is not specific to the things we’ve learned so far. Hardly! It’s a basic architecture for processing and delivering information to users, something nearly every program is responsible for. Our instructor, Avi, gave the example of a restaurant business where the model is the chef and the controller is the waiter, delivering the food. I obsessed with this example for so long and stretched it to its limit (and far beyond,) so I tried to take it from scratch and dig even deeper.



<p align="center"><img src="http://betterexplained.com/wp-content/uploads/rails/mvc-rails.png" alt="Diagram" /></p>

<br>

<h3>Model</h3>
Let’s start with the model. It’s probably where you’ll be spending most of your time, anyway. Models are Ruby classes, and the most logic is going to be in here — more than the other two. They do the heavy lifting and the true processing portion. You want to avoid delegating these out later to something in the controller (that’s what the very concept of MVC is designed to prevent in my opinion). By creating it as independent of the controller as possible, you can have multiple controllers to process as needed. This is also the best place to validate your data as well.

<br>


<h3>Controller</h3>
Next up is controllers. I saw someone describe this as “Dilbert-esque”, and that’s pretty spot on. You remember Dilbert, right? His tie never seemed to stay down against his shirt, probably could've used a tie clip. But that’s not really what tie clips are for anymore, I think they've turned more into a fashion statement at this point. Besides, why does his tie even curve up?




<p align="center"><img src="http://queens.db.toronto.edu/~cmishra/dilbert.gif" alt="Dilbert" /></p>




Anyways, back to the controller. It barks simplistic orders and dictates a lot of the basics of how the program works. Connecting the model to the view, it knows how to do something - but should only know how to do it just well enough to do it correctly. Forcing too much logic in your controller and taking the heavy lifting out of the model is detrimental to your overall program as it is the least abstract way to go about it. A proper controller will never include any database related actions, this needs to be in the model.
<br>
<br>
<h3>View</h3>

Finally, the view is what the user ends up seeing. Using ERB (embedded Ruby), the goal should be to make this as lightweight of a file as possible. You can use HTML and Ruby to render a fantastic output fit for a king! There’s not a whole lot to say about the viewers, but these must be kept simple.

Another diagram I liked a lot was this:

<p align="center"><img src="http://upload.wikimedia.org/wikipedia/commons/a/a0/MVC-Process.svg" alt="Dia2" /></p>


There’s no one right way to draw the diagram, but there are many wrong ways to draw it. None of these are it. With the appropriate planning, you'll have a powerful MVC trio in no time!

<br>

<p align="center"><img src="http://i.imgur.com/DyV6q7u.gif" alt="Sleep" /></p>

(revised 11-10-14)
