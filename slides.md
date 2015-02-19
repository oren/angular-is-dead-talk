# AngularJS is Dead

           .-. __ _ .-.
           |  `  / \  |
           /     '.()--\
          |         '._/
         _| O   _   O |_
         =\    '-'    /=
           '-._____.-'


http://oren.github.io

https://twitter.com/oreng

---
# Angular's original goal

  Misko, Angular's creator: "It’s just that originally, the goal of the system was slightly different.  The goal was for a web designer, somebody who doesn’t necessarily know how to program, to be able to add a bunch of tags into HTML and through static HTML into a dynamic, interactive page."

  http://devchat.tv/js-jabber/109-jsj-dependency-injection-in-javascript-with-vojta-jina-misko-hevery

---
# Good Reads 1/2

* http://www.fse.guru/2-years-with-angular

* Review of Angular: http://www.letscodejavascript.com/v3/blog/2015/01/angular_review

  The author looks at the following criteria: Lock-in, Opinionated architecture, Accidental complexity, Testability and Server-side rendering.

---
# Good Reads - 2/2

* The problem with Angular: http://www.quirksmode.org/blog/archives/2015/01/the_problem_wit.html

* popularity-driven development: http://ferrante.pl/frontend/javascript/popularity-driven-development/

  Mithril's author, Leo, reply here: https://news.ycombinator.com/item?id=8947776

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

* Mithril.js - fast, ajax, router, great docs
* Riot.js - custom tags, router, similar to Angular
* Cycle.js - modular, reactive (events)
* Mercury.js - modular, interactive (similar to cycle but function calls instead of events)

---
# Mithril's Background 1/3

"Mithril is a direct product of working on a multiple-man-year Angular codebase and the pains that arise from such a beast."

---
# Mithril's Background 2/3

The design decisions that went into Mithril to reduce learning curves: http://lhorie.github.io/mithril-presentation-oct-js-tech-night

---
# Mithril's Background 3/3

"It's designed to leverage generic knowledge as much as possible, as opposed to introducing a large amount of framework-specific terminology that no one else uses and that may be out of flavour in 3 years."

---
# Mithril's basics

* size: 5K (1000 lines)
* virtual dom
* commonJS
* promises
* routing
* ajax

---
# Why are templates pure javascript? 1/2

Better error reporting, proper scope/closure/variable shadowing rules, turing completeness (for the purposes of refactoring/abstraction, etc),

---
# Why are templates pure javascript? 2/2

It's friendlier to transpiled language users, it's lintable, it's compressable, it's statically analizable, etc.

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

* https://github.com/eddyystop/mithril-components
* simple single page app with router and animation: http://jsfiddle.net/barney/w8c7b0qw/
* file:///home/oren/projects/mithril-components/public/select2.html

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

* Slides. Intro to Mithril by Leo: http://lhorie.github.io/mithril-presentation-oct-js-tech-night
* isomorphic: https://github.com/StephanHoyer/mithril-node-render
* jsx for Mithril: https://github.com/insin/msx
* Mithril bootstrap modules http://ng-vu.github.io/bootstrap

---
THE END.

                   )\._.,--....,'``.
     .b--.        /;   _.. \   _\  (`._ ,.
    `=,-,-'~~~   `----(,_..'--(,_..'`-.;.'
