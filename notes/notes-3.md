# Week 3

## Pseudo-classes and elements (03-01)

### Pseudo-Classes
- dynamically populated or depend on tree structure
- a:hover


### Types of Pseudo-Classes
- link
    - :link, :visited

- user action
    - active: holding the mouse button on something
    - :hover
    - :focus: usually used to highlight current element in focus (tabbed)

- forms (interfaces)
    - :enabled
    - :checked
    - :disabled, for disabling parts of font until condition is reached (completion usually)

- structural/positional
    - :first-child, :last-child, :nth-child(), :only-child
    - :first-of-type, ...

### Types of Pseudo-element
- textual
    - :first-letter, :first-line
- positional/generated
    - :before, :after
- fragments
    - ::selection




## Transitions (03-02)

### Properties
- transition-property
    - what is changed (size, color, position...)
- transition-duration
    - time it takes to appy it
- transition-timing
    - smooth?
- transition-delay
    - to make it easier so that transitions aren't called by mistake


### Setting Up
1- define the element
2- choose the elements for transition
3- define new values (combined with a pseudo-class)



## Transforms(03-03)

### 2D Transforms
- transform:translate(x,y)
    - takes x,y vector of direction
- rotate
- scale
- skew
- matrix
    - combines all of the 2D transform methods in a command
    - kinda hard to use, try to avoid and use individual transforms

### 3D Transforms
- rotateX(), rotateY(), rotateZ()



## Positioning (03-05)
- four possible positions
    - static
    - relative
    - absolute
    - fixed
- can also be modified by properties tblr (top-bottom-left-right)

### Static (default)
- default value for elements
- place in the next available position
- not affected by tblr


### Relative (similar to static)
- static, with modification by tblr
- default is to itself
- move them from where they would normally go




### Absolute
- ignores other elements
- can cause stacking of elements


### Fixed
- fixes the position in the viewport




### Z-index
- multiple elements can be placed in the same position
- allows modifying the stacking order
- large positive values == on top of other elements






