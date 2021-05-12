# Class-06 Readings: Problem Domain, Objects, and the DOM

## Understanding the Problem Domain is the Hardest Part of Programming-by John Sonmez

The basic premise of this entire article is that if we do not understand the big picture, what is the software/program trying to do-what problem is it solving, then as programmers we're doomed to fail. Maybe not fail, but will spend a significant amout of time flailing around with partial solutions. 

- A few possible COAs:
1. Make the problem domain easier
2. Get better at understanding the problem domain

## Duckett Chapter 3 100-105 Objects.

### What is an Object?
Objects gropu together a set of vairables and functions to create a model of a something you would recognize in the real world. In an object, variables and fuctions take on new names. 
- In an object: variables become known as properties
- In an object: functions become known as methods

The object in the book represents a hotel. It has 5 properites and 1 method. The object is in curly bracess, it is stored in a variable calle hotel. 

`var hotel = {
  name: 'Quay',
  rooms: 40, 
  booked: 25, 
  gym: true, 
  roomTypes: ['twin', 'double', 'suite'],
  '
  The above are properties--the variables.
  'checkAvailability: function() {
    return this.rooms - this.booked;
  }
}`
The checkAvailability string is the method, the function. 

- Literal notation is the easiest and most popular way to create objects. 
- you access the properties or methods on an object uing a dot notation. You can also access properties using square brakets. 

- example: of dot notation
`var hotelName = hotel.name; 
  var roomsFree = hotel.checkAvailability()'

  The period in dot notation is known as the member operator. the property or method on its right is a member of the object on its left. 

- example of square brackets:
`var hotelName = hotel['name'];

## Chapter 5 Document Object Model 183-242
So this looks to be very confusing...
The Document Object Model DOM specifies how browers should create a mode of an HTML page and how JS can access and update the contents of a webpage while it is in the browser window. 
# Neither HTML nor JS, two primary areas:

1. Making a model of the HTML page- uses DOM tree, called and object model because the model DOM Tree is made of objects. 

2. Accessing and changing the HTML page. Sometimes referred to as an Application Programming Interface - API - allows humans to interface with the programs. APIs let programs and scripts to talk to each other. 

# The DOM Tree is a model of a webpage. Consists of four main types of nodes:

1. Document Node-represents the entire page
2. Element Node-H1-H6, p tags
3. Attribute Nodes-not children of the elemnt but part of the element. 
4. Text Nodes-cannot have childred. If an element contains text and onther child element, the child element is not a child of the text node but rather a child of the containing element 

# Working with the DOM Tree. Accessing and updating involve two steps.

1. Locate the node that represents the element you want to work with. Access the elements by DOM queries of traversing the DOM
  1. Select an individual element node
    `getElementById()`
    `querySelector()`
  2. Select multiple elements
    `getElementsByClassName()`
    `getElementsByTagName()`
    `querySelectorAll()`
  3. Traversing between elemenet nodes:
    `parentNode`
    `previousSibling/nextSibling`
    `firstChild/lastChild`

2. Use its text content, child elements, and attributes.This was totally confusing. 
  1. Access/Update text nodes:
    `nodeValue ` 
  2. Work with HTML content
    `innerHTML` page 220
    `textContent` page 216
    create, add, remove nodes by:
    `createElement()`
    `createTextNode()`
    `appendChild()/removeChild()`

# Caching DOM queries
Methods that find elements in the DOM Tree are called DOM queries
  `getElementsById('one');` = DOM Query
  `var itemOne = getElementsById('one');` variable to store result of above DOM query

# Accessing Elements: 



