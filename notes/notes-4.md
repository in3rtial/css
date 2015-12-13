# Week 4

## Styling Tables (04-01)

### Tricks
- alternate colors using tr:nth-child(odd && even) to alternate
- access first and last through tr:last-child>tr:first-child...
- td:active>span{visibility:visible} to make span(and its text) visible on click


## Creating Navingation Menus

### Tricks
- leave size calculations to browser using
	- box-sizing:border-box
- relative url for background imags


## Accessible Navigation
- for blind/low-vision users

### Can't see
- link description that makes sense

### Heading hierarchy
- follow the dom
- h1 > h2 > h3...  headers must be of correct level and tree structure
- never go for aestetics, modify them into the css... wtf


### Off-page headings
- give SR (screen-reader) users a nav aid without cluttering presentation
- use CSS to posiiton headings off-page
.offpage{
	position: absolute;
	left: -1000px;
}
- don't use {display: none; or visibility:hidden}


### Contested status of wether or not use multiple h1 headings
- for and against, might help accessibility and do SEO...


# Creating Navigation Menus 2-3 (04-04)
- .active
- refrain from dropdown navbars as much as possible, way too much usability issues

- nested lists
	- nav li:last-chid{border-right:none;}
	- nav li ul{position:absolute; display:none; width:inherit;}
	- nav li:hover ul{display:block;}
	- makes it display on the right


