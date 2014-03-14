# Frontend Assessment Part 1

### HTML

- What does "semantic markup" mean?

HTML that explains the meaning and/or purpose of the element clearly to the browser and developer. 

- What does a doctype do?

A doctype declaration is not an HTML tag but an instruction to the browser about what HTML version this webpage is written in. Practically, you simply declare <!DOCTYPE html> for HTML5 standard. 

- Explain what standards and standards bodies are and why they are important.

Web standards are rules and guidelines established by the World Wide Web Consortium (W3C) developed to promote consistency in the design code which makes up a web page. Without getting technical, simply it's the guideline for the mark-up language which determines how a web page displays in a visitor's browser window. 

There are a number of standard bodies including ISO, Unicode. 

- What are CSS3 and HTML5? How are they different from previous standards? Why is this important?

They represent the latest version of major changes to CSS stylesheet language and HTML markup language. Both also were marketing campaigns. Both continue to change, as they had before, but major stuff like animation was added to CSS and semantic markup, <canvas> tag, and media support was added to HTML. The combination replaced the need for Flash and made JavaScript redundant in some cases.

### CSS

- What does a CSS reset do and why is it useful?

In the past, browsers had a lot of their own quirks with how they treated CSS, leading to inconsistencies. IE was especially different from the others. CSS reset stylesheets (reset and normalize) to bridge the gap. Today, modern browsers are more consistent across the board, so resets are less necessary if your visitor's browsers are up to date. 

- What is the box model? Draw a picture and label the portions here.

The CSS box model describes the rectangular boxes that are generated for elements in the document tree and laid out according to the visual formatting model, including content, padding, border, margin (in that order). 

- What is the difference between a relative, fixed, absolute, and statically positioned element? Feel free to draw pictures to explain your answer.

static
This keyword let the element use the normal behavior, that is it is laid out in its current position in the flow.  The top, right, bottom, and left properties do not apply.

relative
This keyword lays out all elements as though the element were not positioned, and then adjust the element's position, without changing layout (and thus leaving a gap for the element where it would have been had it not been positioned). The effect of position:relative on table-*-group, table-row, table-column, table-cell, and table-caption elements is undefined.

absolute
Do not leave space for the element. Instead, position it at a specified position relative to its closest positioned ancestor or to the containing block. Absolutely positioned boxes can have margins, they do not collapse with any other margins.

fixed
Do not leave space for the element. Instead, position it at a specified position relative to the screen's viewport and doesn't move when scrolled. When printing, position it at that fixed position on every page.

There is also 'sticky' positioning. 

- What is SASS and why do people use it?

Sass makes CSS fun again. Sass is an extension of CSS3, adding nested rules, variables, mixins, selector inheritance, and more. It’s translated to well-formatted, standard CSS using the command line tool or a web-framework plugin.

SASS is great because it makes writing CSS less redundant, and dare I say it more DRY. It saves you time and energy! 

- Name one feature of SASS and explain why it is helpful.

Mixins. I can set our color palette as mixins ($mainColor = #CCC --> later on in a class -> background-color: $mainColor;) and easy test color schemes!

### JS

- Explain prototypal inheritance.

- What is a closure and how/why would you use one?
Closures are an extension of the concept of scope. With closures, functions have access to variables that were available in the scope where the function was created. If that seems confusing, don’t worry: closures are generally best understood by example.

I use closure to create a new private scope. 

- What is an anonymous function? Give a typical usecase for one.

A JS function without a name. Typical use case applies when you don't need to reference that reference again or is written just for the callback. An anon function can be used to call the function inside the function itself. 

- Describe the difference between 
  - `function Person(){}`
Is a constructor for object Person
  - `var person = Person()`
Is a variable person now points to the object constructor Person
  - `var person = new Person()`
Is a variable person now points to an instance of the Person object

- Explain hoisting.
Instantiating variables (but not defining them) at the top of the document.

- What is the difference between `===` and `==`?
Strict vs normal equality. To be true, values need to be same value and type, while in the case of normal (more lenient equality operator) then it will try and convert different types to the same thing and compare. 
