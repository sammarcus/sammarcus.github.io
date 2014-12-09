---
layout: post
title: "OmniAuth and Users"
date: 2014-12-09 09:30:38 -0500
comments: true
categories:
---

<p align="center"><img src="http://cl.ly/image/2C1l2U0W1G2o/omniauth.png" alt="endpoints" /></p>

OAuth is really cool. Not exactly a groundbreaking statement, but there are many things I have come to appreciate even more now that I have a deeper sense of how they work. When I was first truly putting it to the test in my first project, Identity Crisis, I had a hard time grasping the difference between as merely authorizing a user and the necessity, should your needs require it, to create a mechanism to also have users on your site as well.

OAuth is merely a means to reliably verify someone’s identity on an external service. That’s it. What it’s not is a total solution to facilitate users on you app and manage permissions and control passwords and handle tables and reset forgotten usernames because you don’t need to worry about it because Twitter has it taken care of and everything is easy peazy breazy because OAuth has got it under control. Aha. It is not.

If you want to leverage an external service to interface with a function you are building yourself, OAuth is a great start. But you’ll still need to handle all your users yourself, and simply tack that extra token on should you choose to use it for anything else.It is one less thing you have to do in managing user authentication, but there are still a dozen things left to do before you're done. The Devise gem is a great way to assist in the complexities of securely managing these relationships beyond OAuth.

Alas, nothing is very easy. Twitter was a relatively straightforward example, but the road was a bit bumpier when we tried to kick it into high gear with Uber (double pun intended).

(•_•)

( •_•)>⌐■-■

(⌐■_■)


Knowing we wanted to build something socially powerful enough to move humans around together, Uber was an easy choice when it came to transportation providers. Their service is reliable, the API is robust, the cars were speedy and everything looked like sunny blue sky were ahead. To be clear, OAuth is not an API. OAuth (Open Authorization) has become an extremely common way to access walled APIs, but should not be referred to as an API itself. Basic terminology.

After dipping our toes in the RESTful waters we dove into the deep end to try to finagle Uber to serve us up a fresh token for my user account. It felt a little bit like we were going down a dark tunnel with no flashlight, so I relied on the Mac app Paw to familiarize myself with the raw traffic we were sending. It was also really helpful since it parsed JSON all in one swoop. We ended up using the OmniAuth gem, which includes basic OAuth strategies all under one roof. Once we finally landed on the correct params to send over (all over HTTPS, of course, because you already knew that you have to force Heroku to interact securely and not spend an hour panicking that the whole service strategy has to be scrapped), we got our token through redirect and stashed it aside for safekeeping. Yep, that’s right. We just used that as a means to log into our app. This way we never ask for a password! Uber can handle that drama. Thanks Uber.

<p align="center"><img src="http://cl.ly/image/3L1S2B1i122H/Image%202014-12-09%20at%209.40.11%20AM.png" alt="screenshot" /></p>


 So now that we know WHO they are through a means of a token, and we know WHAT they are since we have them as a user through Devise, we can make snazzy requests on their behalf. Whoop whoop. Because they granted us permission through OAuth, we have some capability to act on their behalf and can perform actions that Uber has scoped us with the appropriate permission to do so. More on those difficulties in round 2.
