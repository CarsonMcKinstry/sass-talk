# What is Sass

It is a preprocessor for CSS. It allows you to write your CSS in a much more concise way, and adds some functionality for keeping your CSS as DRY as possible.

## Two syntaxes

There are two syntaxes

* Sass ( Syntactically awesome stylesheets )- syntactically significant white space
* SCSS (Sassy CSS)- Looks and feels more like CSS


## Nesting

This is the most used part of Sass. This allows you to get as specific as possible without having to chain selectors. Normal nested elements simply require a tab in and the selector. Sibling selectors, ex: `<button class="btn btn-submit"></button>` require an ampersand before the second selector.

## Variables

Variables do exactly what you would think they do, store values. Anything that you want can be stored in a variable. Most commonly, you will store colors, screen sizes, font stacks, etc.

## mixins

These are basically functions for CSS. They take in a value and output it the same way any other function would. A very common use is for prefixing your selectors. You can also use them to do just about anything you would in another language

## extends

These are similar to mixins. These are used instead of mixins when you have one style aspect you want in multiple places, but it doesn't need to be variable. One rule of thumb is that if you aren't using a variable in a mixin, it needs to be an extend. They are normally prefixed by a percent sign, but class selectors work as well. (Best practice is the percent sign);

## imports and partials

SASS supports partials, which are files containing snippets of your code. This allows for your code to be less verbose and more concise, and increases the overall maintainability of the code (variables in one folder/file, mixins in another, etc.).

## Operators
There are a bunch of them, and they let you do math in Sass `+`, `-`, `*`, `/`, and `%`. They let you do math in Sass and are actually use in Bootstrap to create the grid system.

## Other features

- Nested @media queries
- @if, @for, @each, and @while

## compiling

This can be done a few different ways. You can use the SASS compiler itself, or use the `node-sass` npm package. I've included a package.json file in this talk's repo that contains the package as well as 4 scripts, for building and watching Sass and scss. It can be installed globally as well, but that is better handled by the actual SASS compiler.
