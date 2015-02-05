# Angular.js is Dead

(run the slides with `npm start`)

http://oren.github.io

https://twitter.com/oreng

---
# Angular's original goal

  From an interview with Misko, Angular's creator:
  "It’s just that originally, the goal of the system was slightly different. The goal was for a web designer, somebody who doesn’t necessarily know how to program, to be able to add a bunch of tags into HTML and through static HTML into a dynamic, interactive page."

  http://devchat.tv/js-jabber/109-jsj-dependency-injection-in-javascript-with-vojta-jina-misko-hevery

---
# Good Reads

* http://www.fse.guru/2-years-with-angular

* Review of Angular: http://www.letscodejavascript.com/v3/blog/2015/01/angular_review
  The author looks at the following criteria: Lock-in, Opinionated architecture, Accidental complexity, Testability and Server-side rendering.

* The problem with Angular: http://www.quirksmode.org/blog/archives/2015/01/the_problem_wit.html

* popularity-driven development: http://ferrante.pl/frontend/javascript/popularity-driven-development/
  mithril's author, Leo: https://news.ycombinator.com/item?id=8947776

* http://lhorie.github.io/mithril-blog/lessons-learned-from-angular.html

---
# Thriving community

* http://ihateangular.com/

---
# React + Flux

Virtual Dom, Unidirectional apps

https://gist.github.com/alexmingoia/4db967e5aeb31d84847c#what-is-a-unidirectional-app

---
# Micro virtual-dom frameworks

* Mithril.js - ajax, router
* Riot.js - custom tags, router, similar to Angular
* Mercury.js - modular, interactive (similar to cycle but function calls instead of events)
* Cycle.js - modular, reactive (events)

---
# Mithril's Background

"Mithril is a direct product of working on a multiple-man-year Angular codebase and the pains that arise from such a beast."

I wrote about that here http://lhorie.github.io/mithril-blog/lessons-learned-from-angular.html
On a related topic, I talk about complexity walls (the idea of code that outgrows a framework's zone of comfort) http://lhorie.github.io/mithril-blog/decreasing-cognitive-load.html
and there are slides for a presentation I gave a while back that talks about the design decisions that went into Mithril to reduce learning curves. http://lhorie.github.io/mithril-presentation-oct-js-tech-night

Mithril might be worth looking into. It's similar to React in terms of providing a unidirectional data flow pattern for code organization, and it comes with a few other useful tools out of the box (e.g. routing, ajax, promises), despite being smaller in terms of byte count.
It's designed to leverage generic knowledge as much as possible, as opposed to introducing a large amount of framework-specific terminology that no one else uses and that may be out of flavour in 3 years.
I've heard people say they were able to get up and running in less than an hour, so even if you don't ultimately use it, I think it's worth investing some time into looking into it.

---
# Mithril's basics

* size: 16K
* virtual dom
* commonJS
* promises
* routing
* ajax

---
# Why are templates pure javascript?

better error reporting, proper scope/closure/variable shadowing rules, turing completeness (for the purposes of refactoring/abstraction, etc), it's friendlier to transpiled language users, it's lintable, it's compressable, it's statically analizable, etc.
https://news.ycombinator.com/item?id=8973867

---
# API design

What made jquery so successful?

```js
//set the color of one element
$("#foo").css("color", "red")

//get the color
$("#foo").css("color")

//set the color on many elements
$("h1").css("color", "red")
```
---
# Some examples

Not sure what's the best examples to show.
I prefer to show real modules that are easy to understand -
something like login module, complete website with multiple modules, etc

---
# What is a Mithril module?

```js
{ view: function() {} }
```

---
# What is a Mithril module?

```js
{ view: function() { return m("div") } }
```

---
# Links

* isomorphic: https://github.com/StephanHoyer/mithril-node-render
* boilerplate: https://github.com/velveteer/mithril-boilerplate
* jsx for mithril: https://github.com/insin/msx
* simple single page app with animation: http://jsfiddle.net/barney/w8c7b0qw/

---
THE END.
