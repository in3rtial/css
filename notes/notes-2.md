# Week 2

## Box model (2-01)

### Borders
- colors the area around
- style must be specified
- allows to work easily with elements and understand behavior
- can specify individul styles (1-4 values in px)



### Margin
- space outside the border
- positive or negative margin (further or closer)
- used to center elements
    - margin: 0 auto;
    - will only work if:
      - display:block;
      - not float
      - element doesn't have a fixed or absolute position
      - width is not auto

### Padding
- between the elements and the border



### Details
- actual width is width or height + 2*(borders + margin + padding)
    - since they are 

### Box-sizing
- takes the math out
    - content-box: default additive
    - border-box: width takes content, padding and border into consideration


### Measurements
- absolute
    - px, mm, cm, pt
- fluid (relative to surrounding elements)
    - %, vw, vh
    - em  (fonts)
    - rem (fonts): current size of root element



### Putting h2 next to each other
- use the inline-block and width 40%



## Code together (02-02)

### Summary
- when want to put divs next to each other, inline-block and with setting... as before
- float:left; used to make sections float around each others
- clear:both; when don't want anything floating around element


## Links and lists (02-03)
- don't style links as buttons, never
- don't style them so they aren't link-looking (e.g. for screen readers)


### Link states
- a:link
- a:active: adds a border when clicking, goes away after click
- a:hover
- a:focus: useful for people "tabbing" through a page
- a:visited
- rule precedence
    - a:hover after a:link
    - a:visitide and a:active after a:hover


### Lists
- can add redundancy in choices (like fonts, if first not available, next is tried until default)


## Advanced Selectors (02-04)


### CSS selectors
- descendant selectors (nav a)
    - style all of the anchors in the nav tree, no matter the distance

- child selectors(nav > a)
    - more constraining
    - anchor element must be a direct child of the nav, no intermediate

- adjacent siblings (h1 + ol)
    - elements must be descendant of the same parent (siblings)


### Id selectors
- can identify single element in the DOM
- getting out of CSS currently
- # symbol


### Class selectors
- part of a special class of items
- .symbol


### Class and id differences
- symbols
- id is unique, class will be reused



### Universal Selector
- *
- useful for debugging


### Attribute Selectors
- a[href="info.html"]
- adds more refinement
- searches the DOM for features such as
    - all images using gif files
    - all images with empty alt text !!!
    - all links to .gov sites
- uses operators (regex pretty much)



### Operators
    - ^: match beginning exactly
        - a[href^="http://umich"]
    - $: match the end exactly
        -img[src$=".png"]
    - *: contains substring
      - a[href*="umich"]


### Pseudo-Classes
- a:link
- a:hover ...



### Pseudo-Elements
- used to style specified parts of an element
    - the first letter, line
    - insert content before or after the content of an element
- ::first-line pseudo-element is used to add a special style to the first line of a text.

### Scope Expansion
- can combine elements with a comma
    - p, h1, main...
- multiple rules for a selector
    - conflict? use the one processed most recently unless a rules has !important

### Can override with own stylesheet
- override decisions of copied css







## Browser capabilities (02-05)
- variable adherence to new HTML5 standard
- use default style sheet


### Browser Prefixes
- -webkit-: android, chrome, ios ,safari
- -moz-: Firefox
- -ms-: IE
- -o-: Opera


### Often Unsupported Properties
- column-count
- border-radius
- gradient
- sites such as caniuse.com will tell you when you need the prefixes


## Designing For Accessibility (02-07)
- KISS principle
- content in .html
    - keep in mind that not every user is a visual user

### POUR guideline
- perceivable
    - always img with alt
    - captions and transcripts for audio and video
    - correct semantic markup (nav, figure)
    - good color contrast
- operable
    - content that blinks, flashes, can cause seizures
    - functionality from keyboard only
    - users have control over timingand limits
    - provide ways to help users navigate and find content easily
- understandable
    - plain language
    - text supplemented with information where necessary (use good universal design)
    - navigation, information structure are discernable and consistent
    - mage pages operate in predictable ways
    - make it easy to correct mistakes
- robust
    - portable over many technologies (responsive design)
    - syntax errors which are okay might influence assistive technologies (use w3c and wave.webaim)

### Summary
- use tools
- get people to evaluate
- keep to technologies with accessibility in mind



