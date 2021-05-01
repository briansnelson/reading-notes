# Day 3 Reading HTML Lists, Control Flow with JS, & CSS Box Model

## Lists from Chapter 3 of Duckett's HTML/CSS book

### Lists for HTML are in three types

1. *Ordered lists* of which this happens to be one, it is numbered
2. *Unordered lists* which begin with a bullet point
3. *Definition lists* are sets of terms along with definitions.

**Another way to describe the same lists are:**

- Numbered lists
- bullet lists
- definitions

Here I'm going to try to used a code block so I can show what I mean by using these particular tags in HTML.
```
<ol> is an ordered or numbered list
<ul> is an unordered list or bullet list
<li> is how you code the specific lists, the ol and ul are opening and closing tags for the previous lists. Both ordered and unordered us <li>
<dl> is the opening tag for definitions <dt> contains the term and <dd> contains the definition.
```

## Boxes

This chapter discusses

- Controlling the size of boxes
- Box model for borders, margin and padding
- Displaying and hiding boxes

**BLUF**  *Bottom Line Up Front*

- CSS treats each HTML element as if it has its own box

- CSS can be used to control the dimensions of a box

- This control includes borders, margins, and padding within box.

- Possible to hide elements using the diplay and visibility properties

- Block-level boxes can be made into inline boxes, and vise versa

### Box Dimensions

A default box is sized to fit the contents, can use width and height to set properites. 

Most popular wasy to specify box size are to use:

- pixels, percentages, or ems. Percentages are either relative to size of page, or the box in which working box sits. Ems are based on size of text within box.

- Limiting Width: min-width and max-width example in book used tags for text table and text data tr and td

- limiting height is similar principles as width

- overflow has two options: hidden or scroll. Self-evident

1. Borders-every box has a border if not visible it is set to 0. Separates edge of box from another

- border-width top: thin,   medium, thick and top/right/bottom/left. use px or pixels

- border style: solid, dotted, dashed, double, groove, many more

- border color: each side

- shorthand border: putting all CSS into one command


2. Margin- margins sit outside the edge of border. Can set width of margin to create a gap between borders of adjacent boxes. Similar pattern as border.

3. Padding-similar to matting in a photo frame. Similar to border all sides, etc

Using these three help create white space and vertical margin, easier to read and more elegant

- Centering conent by using text align

- IE6 box model: by using DOCTYPE, you over ride IE6 standard box padding and margin

- Inline/block: you can reverse these or combine with inline-block or none

- hiding boxes- do this with visability - and example is a product or service that isn't available.

### CSS3 has super sexy

1. Border images
2. Box Shadows
3. Rounded corners
4. Ellipical shapes

## JS Chapter 2 Basic JS and Chapter 4 Decisions and Loops

## Arrays:

An array is a special type of variable. It stores a list of values. 

- Array literal: The values are assigned inside a pair of square brackets, values separated by comma

- Array constructor uses parenthesis and values separated by comma. 

## Decisions & Loops

1. Decisions: using the results of evaluations to decide which path script should follow

- two components to a decision: An expression is evaluated, which returns a value. A conditional statement say what to do in a given situation. 

2. Loops: times when want to perform same set of steps repeatedly. 

All of this is to answer yes or no, true or false. The scripts must be written to be binary in options. 

### If...else statements:

This checks a condition. If resolved as true, the first code block is executed. If the condition resolves as false, the second code block is executed. 

### Switch Statements
Starts with a variable called a switch value. Each case indicates a possible value for this variable and the code that should rune if the variable matches that value.

### Type coercion and weak typing

String is for text, number is number, boolean is t/f, null is empty value, undefined has been declared but not assigned. Because of type coersion strict equals is better ===

### Truthy and falsy values
So, I don't really udnerstand this.
Falsy values can be treated as zero, truthy values can be treated as 1. Both are treated as if they were false or as if they were true.

### Checking Eqaulity and Existance. 
A unary operator returns a result with just one operand. 

### Short Circuit values:
logical operators are processed left to right. They short circuit or stop as soon as they have a result - even if not necessarily true of false.

Logical operators will not always return true or false because:

- they return a value that stopped processing

- that value might have been treated as truthy or falsy although it was not Boolean.

## Loops--didn't like this in 102. 
Loops check a condition. It if returns true, a code block will run, keeps running until a condition returns false. Three common types of loops:

1. For loops: Run a code for a specific number of times, this is also most common

2. While loops: if you do not know how many times a code should run use a counter

3. Do While similar to above EXCEPT it will always run the statements inside curly braces at least once even if condition evaluates to false.

Loops are composed of keyword like for: a condition, opening curly brackets, the code to execute, then closing curly bracket. 

Break it down further:
initialization: condition: update.
var i = 0
condition i < 10; 
update i++

