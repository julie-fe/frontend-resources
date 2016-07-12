# JavaScript/TypeScript
In JavaScript/TypeScript we use the CamelCase Syntax    
* [Typescript Handbook](http://www.typescriptlang.org/docs/)

**Variables**   
Variables start with a lowercase char
```typescript
let myVar = 1;
let mySecondVar = myVar;
```
**Strings**  
Strings should always be written with a single quote or the new char for Template Strings.
Don't use double quotes for declaring strings.
[Template String documentation on babeljs.io](https://babeljs.io/docs/learn-es2015/#template-strings)
```typescript
// bad
let bad = "dont do that";

// good
let goodString = 'much better :)';

// also fine
let templateString = `This string is ${goodString}`;
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

**Functions & Methods** 
Functions, Methods and Parameters start with a lowercase char.
Only Parameters which are Class Definition are written with a leading uppercase char.
```typescript
// function
function myFunc() {
}

// function with param
function mySecondFunc(param1: string) {
}

class MyClass {
  constructor(someParam: number) {
  }
  
  // methods  
  method(anotherParam: string) {
  }
  
  wildMethod() {
  }
}
```

**Documentation & Comments**    
TODO