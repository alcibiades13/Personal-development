# Notes from dev talks and tutorials


## Eric Elliott -  Fluent 2014 JavaScript Talk - Static Types are Overrated 

- type correctness does not guarantee program correctness!
- you should be using automated testing for every program
- use *jshint* - variable name typos, underfined variables, unused variables, cyclomatic complexity
- *tern.js* - autocompletion on variables and properties, function argument hints...
- *trace.gl* - for debugging - records every single function call, traces every value as it flows through program
- *dominators view* in chrome dev tools - making sure objects are being garbage collected
- automated testing - keep your modules small and independent
- write tests first
- jsdoc static analysis - tern can parse jsdoc for type hints - DocBlockr SublimeText
- you can use .map() on strings


## Janne Jul Jensen - UI/UX techniques and guidelines

- Simple and natural dialogue
- Speak the user's language
- Minimize memory load (let computer remember, not the user)
- Use constructive error messages
- Support recall
- Make clear exits (never get the user into a corner they don't know how to get out from)
- Make shortcuts
- Give feedback (always tell the user what's going on)
- Prevent errors (anticipate where they can appear)
- Thrive for consistency


## Eric Elliot - The Two Pillars of JavaScript: How to Escape the 7th Circle of Hell

- Once Upon a Time. I was trapped in the darkness. I was blind.
- JavaScript offers something other languages lack: **Freedom!**
- JavaScript popularized two paradigms which are extremely important for the evolution of programming:
	-- Prototypal Inheritance (objects without classes, and prototype delegation, aka OLOO — Objects Linking to Other Objects), and
	-- Functional Programming (enabled by lambdas with closure)
- I like to call these paradigms the two pillars of JavaScript
- JavaScript is pretty good at letting you code poorly if you don’t bother to learn it properly
- If you’re creating constructor functions and inheriting from them, you haven’t learned JavaScript
- “Those who are not aware they are walking in darkness will never seek the light.” ~ Bruce Lee
- Constructors violate the open/closed principle because they couple all callers to the details of how your object gets instantiated.
- In JavaScript, factory functions are simply constructor functions minus the `new` requirement, global pollution danger and awkward limitations (including that annoying initial capitalized letter convention).
- JavaScript doesn’t need constructor functions because any function can return a new object.
- “The problem with object-oriented languages is they’ve got all this implicit environment that they carry around with them. You wanted a banana but what you got was a gorilla holding the banana and the entire jungle.” ~ Joe Armstrong
- Problems: The Gorilla / Banana problem, The Tight Coupling Problem, The Duplication by Necessity Problem
- The `class` keyword will probably be the most harmful feature in JavaScript.
- Other good alternatives include making better use of JavaScript modules as an alternative to inheritance (I recommend npm and ES6 modules with Browserify or WebPack), or simply cloning objects by copying properties from a source object to a new object (e.g. `Object.assign()`, `$.extend()`, `_.extend()`, etc…).


## 5 web design predictions for 2016 - Barrett Self

1. Rich animation
	- It’s no longer the goal to merely impress a user visually while offering great content. These days, users want to be ENTERTAINED! Enter animation.

	- Loading animations - Utilized to entertain and occupy users while a site transitions into a new page or feature. 
	- Hover Animations – Used to offer insight on an image, tab or graphic’s function. 
	- Motion Animations – The easiest way to grab a user’s attention? MOTION! Motion animation can be a GREAT marketing tool when done right.
	- Smooth Scrolling – Allows a seamless transition between pages and site elements. Besides being fun, this trend also allows users to go at their own pace and reduces eye-fatigue.

2. Minimalism
	- When it comes to web design, less is often more. There are many reasons for this: chiefly, it allows a site to be bandwidth-conscious while ensuring the user isn’t overwhelmed. But on top of that, the simplicity of such a design can be stunning.
	- It would seem that this trend is in opposition to Rich Animation, but on the contrary. When used most effectively, rich animation is applied to a minimalistic design. This way, the focus stays on the animation and the user isn’t distracted by unnecessary information.
	- One specific form of minimalism are flat designs. Which oh, by the way, have SKYROCKETED in 2015! For those of you who are already masters of flat design, good news: their presence is only going to expand in the coming year.

3. Graphic text
	- Type placed within a graphic, positioned over an image, on top of a color pattern… seem like a bit much? In some cases, BUT, if you have a good eye for design – always striving for readability, complimentary colors, and proper focal points – you can transform these dynamic elements into a cohesive experience (one that the end users will thank you for).

4. Apps, apps, and more apps!
	- To say that the app business is booming is an understatement.
	- With app integration into web browers, operating systems, and website templates, the trend will only continue to grow. Unfortunately, its not all roses when it comes to the app surge.
	- An understanding of the available and trending apps that are out there is a must, but their widespread incorporation? Not so much.
	- Tred lightly with this trend!

5. Intro pages
	- An introductory page – or splash page – that precedes a homepage has been around for several years now (especially for sites with a product to sell).
	- The concept makes sense: the user obviously is interested in the site’s purpose, so why not show them what you offer right off the bat? For an author selling a book, it’s perfect. For an online magazine looking for subscribers, just as good.
	- Be wary of overusing this trend, but, as long as you stick to the two rules of sales (be concise and provoke action!), you should be fine!


## Rules of great form design (Adi Purdila)

- Organize the form properly
- Show helper text
- Use the correct input type and length
- Provide clear labels for each field
- Let users know about the expected input format
- Give feedback
- Think about users on mobile devices
- Don't ask for unnecessary information

## Most popular web fonts with sans serif and serif typefaces (dramathic typography)

- Sans Serif
	1. Proxima Nova
	2. Futura
	3. Open Sans
	4. Helvetica Neue
	5. Avenir
	6. Montserrat

- Serif
	1. Caslon
	2. Garamond
	3. Freight Text
	4. Minion
	5. FF Meta Serif

