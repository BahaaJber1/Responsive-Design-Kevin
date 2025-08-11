# Respoinsive Design by Kevin Powell 

## Here I'll be putting all the extra information about the challenges or the things I learn

### 1. Challenge 01

This challenge talks about how the web is **ALREADY** respoinsive, we just make it behave otherwise using css.
And here's the problem if you want to keep things responsive avoide using units like **px**, instead use **[%, em, rem]**, and **DON'T** use heights for fun just keep the content take its height. 

- EM & REM

The main difference between the two units is R stands for **Root** which is the html and by defaults its *16px*, when sitting a size for 
*1rem* for ex, the element gets exactly **16px** but when using *em* its relative to the direct parent size no the root.

- Why you **shouldn't** set font-size using em

The problem is when it starts cascading, ex: 

```
<ul> <li>item</li> </ul>
    <ul> <li>item 2</li> <ul>
        <ul> <li>item 3</li> <ul>
```
So if the first unordered list has a font-size of 1.5em, **the next will have 1.5em * 1.5em and so on.**
