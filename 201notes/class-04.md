# Reading Notes: HTML Links, JS Functions, CSS Layout

The following notes are all from Duckett's HTML & JS books.

## Chapter 4 Links

### Links Summary

- Links are created using the `<a>` element.
- The `<a>` element uses the `href` attribute to indicate the page linked
- When linking to a page within own site, best to use relative links rather than qualified URLs.
- Possible to create links to open email programs with an addres in the "to" field
- You can use the id attribute to target elements within a page that can be linked. 

## Chapter 15: Layout

### Layout Summary

- `<div>` elements are ofetn used as containing elements to group together sections of a page.
- Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning
- The float property moves content to the left or right of the page and can be sued to create multi-column layouts. *floated items require a defined width*
- Pages can be fixed width or liquid *stretchy* layouts.
- Designers keep pages within 960-1000 pixels wide and idicate what the site is about within the top 600 pixels *todemonstrate its relevance without scrooling*
- Grids help create professional and flexible designs.
- CSS Frameworks 
provide rules for common tasks.
- You can multiple CSS files in one page

## Chapter 3 Functions

- What is a function? Series of statements grouped together because they perform a specfic task. These are asked to perform by 'calling the funciton' This function stores the statements so all one needs to do is call the script at the appropriate place.
- Method is same as fuction only methods are created inside *and are part of* an object.
- Objects models of the world made up of properties and methods.
- Built-In Objects: These are built into websites, like a tool kit.

- Declaring a function. You create a function by naming it and then write the statements needed to achieve task inside moustache brackets: `function sayHello() {
  document.write('Hello!');
}`

- Calling a Function. This is what is sexy. Now, after haven written all the complicated tasks inside the moustace brackets--you can just 'call' the function with one line of code: `sayHello();`
- Sometimes functions need specific info to perform a task. This info is called a parameter, act like variables: `function get Area(width, height) {
  return width * height;
}`
When you call this type of function, you need to specify th values: `getArea(3,5);`
- single value of function example: `function get Area(width, height) {
  return width * height;
  return area;
}`
In this example, the area, value of width x height is calculated and delivered
- multiple values:
`fuction getSize(width, height, depth) {
  var area = width * height;
  var volume = width * height * depth;
  var sizes = [area, volume];
  return sizes;
}`
- hidden functions called function expressions `var area = function(width, height) {
  return width * height;

};
var size = area(3,4);`

- variable scope and how memory & vairables work
This is interesting. If you create a variable using the var keyword within a function, it can only be used within the function. It is a **local** variable or **function-level** variable. It is said to have **local scope** or **function-level scope**. It is limited to the function
If the function runs twice, the variable can have different values each time AND
two different functions can use varaibles with the same name without naming conflicts.

- How memory & variables work. Global variables are heavier, use more memory. Local variables are light, only brought 'to mind' when the function is being executed. 
It seems to me that using global variables could impact the speed/usability of one's webpage. 


## 6 reasons pair programming from CodeFellows author Allie Grampa 

1. greater efficiency
2. engaged collaboration
3. learning from fellow students
4. social skills
5. job interview skills/practice
6. work enviornment readiness
