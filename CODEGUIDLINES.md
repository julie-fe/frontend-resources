# CODE GUIDLINES

## Table of Contents
- [CSS](#css)
  - [In short](#in-short)
  - [Links](#links)
- [JavaScript/Typescript](#css)

## CSS

### In short

**Blocks**
```css
.block {
  // your code
}
.my-block {
  // your code
}
```    
**Block Modifiers**
```css
.block--modifier {
  // your code
}
.my-block--modifier {
  // your code
}
```

**Block Elements**
```css
.block__element {
  // your code
}
.my-block__element {
  // your code
}
.my-block__my-element {
  // your code
}
```
**Block Element Modifier**
```css
.block__element--modifier {
  // your code
}
.my-block__element--modifier {
  // your code
}
.my-block__my-element--modifier {
  // your code
}
```

### Links
- [SASS/SCSS](http://sass-lang.com/guide) We use SCSS
- [SMACSS](https://smacss.com/) Scalable and Modular Architecture for CSS.
- [BEM](http://getbem.com/) Block Element Modifier


## JavaScript/TypeScript
In JavaScript/TypeScript we use the CamelCase Syntax    
* [Typescript Handbook](http://www.typescriptlang.org/docs/handbook/)

**Variables**   
Variables start with a lowercase char
```typescript
let myVar = 1;
let mySecondVar = myVar;
```
**Classes and instances**   
Classes start with a uppercase char, instances with a lowercase char like variables (they are variables)    
[Classes auf typescriptlang.org](http://www.typescriptlang.org/docs/handbook/classes.html)
```typescript
// class
class MyClass {
}

// instance
let myClass = new MyClass();
```

**Interfaces**    
Interfaces should start with an uppercase char.   
For better readability prepend a leading uppercase "I" to the interface name.    
[Interfaces auf typescriptlang.org](http://www.typescriptlang.org/docs/handbook/interfaces.html)
```typescript
// good
interface MyInterface {
}

// better
interface IMyInterface {
}
```
