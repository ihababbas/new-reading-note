# Class 03

> ## lists and keys
### What does .map() return?

    lists of elements 

### If I want to loop through an array and display each value in JSX, how do I do that in React?
     we return a <li> element for each item. Finally, we assign the resulting array of elements to listItems Then, we can include the entire listItems array inside a <ul> element.
### Each list item needs a unique ____.
    A “key”

### What is the purpose of a key?
    is a special string attribute you need to include when creating lists of elements. We’ll discuss why it’s important in the next section.

---
> ## The Spread Operator

### What is the spread operator?
    is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.
### List 4 things that the spread operator can do.
    1. Copying an array
    2. Concatenating or combining arrays
    3. Using Math functions
    4.Using an array as arguments
### Give an example of using the spread operator to combine two arrays.
     console.log 
### Give an example of using the spread operator to add a new item to an array.
    arrayName[index]
### Give an example of using the spread operator to combine two objects into one.
     newObj = {obj1 ,obj2}
---
> ## React - How to Pass Functions between Components

### In the video, what is the first step that the developer does to pass functions between components?
     Knowing the elemants thats need to pass as prop and the elemants thats need to pass as stats 
   
### In your own words, what does the increment function do?
    By using the map function loop through to all elemants searching for spicifiec one and before that we decide to use stats becuse it's a change verabile 
### How can you pass a method from a parent component into a child component?
     Props and Stats
### How does the child component invoke a method that was passed to it from a parent component?
       in depeds on the type of the child component either a fix elemnat or changable
---
## Things I want to know more about
  loop throught objects and update it