---
layout: post
title: "Packages on Packages on Packages"
date: 2014-10-23 09:32:02 -0400
comments: true
categories: Flatiron School
---

Inspired by <a href="http://tomcohenno.github.io/blog/2014/10/20/rrrrrrrspec/">Tom’s RubyTest package add on post</a>, I went on a hunt to find other cool additions that might make our day to day tasks even easier. I did not return from the hunt empty handed! Here are four that particularly stood out to me:

<p><img src="http://cl.ly/image/3o362H3s1d3h/Image%202014-10-23%20at%209.43.35%20AM.png" alt="Meme" /></p>



<h2>Git Package</h2>
<a href="https://github.com/kemayo/sublime-text-git/wiki">Git Install Details</a>

Github is the backbone behind collaborative software development, making this service a fairly language agnostic tool relevant to everyone. The aptly named package “Git” for Sublime ties in core functions directly within the text editor. Even though I haven't reached the point where I’m cloning other people’s code outside the school to work on, it still includes basic functions that allow you to bypass terminal and work directly inside Sublime.

<p><img src="http://cl.ly/image/2B0M1Z332h3h/Image%202014-10-23%20at%209.44.27%20AM.png" alt="List" /></p>

An especially useful option is Quick Commit, which simultaneously stages your commit as well. Note that you can type in your commit message in a special dialog option that appears. Current Git branch status is displayed at the bottom of the status bar at all times. Finally, you can push as well.

<p><img src="http://cl.ly/image/1O1I2f0I1A2S/Image%202014-10-23%20at%209.45.24%20AM.png" alt="GitMessage" /></p>

<p><img src="http://cl.ly/image/320c3v0N2L2x/Image%202014-10-23%20at%209.45.46%20AM.png" alt="GitStatus" /></p>

<h2>SublimeLinter Package:</h2>
<a href="https://sublime.wbond.net/packages/SublimeLinter">SublimeLinter Package Details</a>

For those who may be syntax challenged, two Packages stood out as particularly useful. SublimeLinter and SublimeCodeIntel have both proved useful and timesaving additions to my Package library.

Linting, as described by Wikipedia:
<blockquote><p>In computer programming, lint was the name originally given to a particular program that flagged some suspicious and non-portable constructs (likely to be bugs) in C language source code. The term is now applied generically to tools that flag suspicious usage in software written in any computer language. The term lint-like behavior is sometimes applied to the process of flagging suspicious language usage. Lint-like tools generally perform static analysis of source code.</p></blockquote>
As all of my past tablemates can attest to, I became wildly skilled at failing to end my method definitions. Of course, this would cause the entire program to produce an error. Linting packages for Sublime (there are many) take a language-specific Linter and referbce those while checking your code for potential errors in real time. Like everything in Sublime, options to customize are abound.

Because the default evaluates code in realtime as you type (similar to spellcheck), experienced users may find this especially distracting as there will always be errors before you finish your line. You can change to have it delay to avoid this. SublimeLinter shows both warnings and errors, shown respectively below.

<p><img src="http://cl.ly/image/3m3D1j3y1O11/Image%202014-10-23%20at%209.46.12%20AM.png" alt="LintDwarves" /></p>
<p><img src="http://cl.ly/image/461H2T0e1X0G/Image%202014-10-23%20at%209.47.38%20AM.png" alt="LintLast" /></p>


<h2>SublimeCodeIntel Package:</h2>
<a href="https://sublime.wbond.net/packages/SublimeCodeIntel">SublimeCodeIntel Package Details</a>

On our first day we installed Ruby specific add ons, which generally autocomplete Ruby syntax particularly well. Another is CodeIntel, which I have come to prefer as it saves time by offering cookie cutter methods with autocomplete.

<p><img src="http://cl.ly/image/1n3K34383M1w/Image%202014-10-23%20at%209.46.32%20AM.png" alt="Intel1" /></p>
<p><img src="http://cl.ly/image/1z2Q0j0E3I1g/Image%202014-10-23%20at%209.46.55%20AM.png" alt="Intel2" /></p>

<h2>Terminal Package:</h2>
<a href="https://sublime.wbond.net/packages/Terminal">Terminal Package Details</a>

Finally, Terminal by Will Bond (the same person who made the famous Package Control) is a super simple option to open the current Sublime file in Terminal, auto navigating to the appropriate directory with a cd command in the background.

All of these are compatible with both Sublime Text 2 and Sublime Text 3 and can be installed with Package Control.
