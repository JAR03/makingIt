---
layout: post
title:  "From Text-Adventure Game to Design Patterns"
date:   2016-07-17
categories: update
---
Having and working on projects seems to be the gateway for aspiring web developers to gain any traction or recognition in the field. But coming up with a project idea isn't that cut-and-dry. When you're starting off learning the trifecta of web development (CSS, HTML, and javaScript), the usual assignments include some form of to-do list or maybe using an API to create a weather app. Things of these sorts. By all means I'm not saying these aren't practical and education and fun, but making apps of these sorts, in my opinion, won't really separate myself from the masses.

For a really simply project, I decided I'd work on a text-adventure game (which sounds a bit hypocritical considering this too isn't all that impressive). My favorite part of any project is the design work. Thinking of how parts will interact with each other. When you first encounter this type of program, you'll usually be introduced to logic through if-else/switch-case statements. But I wanted something a bit more "professional". So I started with the idea of having an object store the information of a possible scene (i.e., you just encountered a bear. What do you do?) with the possible choices (ie., "fight", "run") and following scenes based off the choice made. This could be demonstrated as such.

var opening_scene = {
	dialog:"You've just encountered a bear. What will you do?",
	choices: {
		option1: {
			fight: fight_scene
		},
		option2: { 
			run: escape_scene
		}
	}
};  

It makes sense to me. And there in lies the "problem", if you will. Although a text-adventure game on the surface seems simple enough, this is really a good example in which a design pattern could be used. Through some research, the one that most resembles this form of logic is the strategy pattern.

In my quest to learn more about the strategy pattern, the prevailing words of wisdom were there that in order to truly understand design patterns, you'd have to learn more about test-driven development, or TDD. Full-stop. This is where my joy for programming and learning comes from. When you think you have a potential solution, you're opened up to a whole new world of thinking and methodologies.

So to make a really long story short, that's where I'm currently at. I'm learning how to use Mocha and Chai in relation to TDD and behavioral-driven developement (BDD). This is going to involve unit testing and a whole slew of technologies that I've never heard, and I can't wait! :)

As a side-note, books that I'm currently going through: 
Secrets of the javaScript Ninja
javaScript -  The Good Parts
javaScript for Web Developers

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
