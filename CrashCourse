# Initial Overview
[Guide Used for this crash course](https://www.youtube.com/watch?v=jrKcJxF0lAU)

TypeScript is a superset language

for example in JS, you can do the following statement
```JavaScript
let name = "laith harb";
```
but in TypeScript you will have to specify the type of the variables
```TypeScript
let name:string = "laith harb"
```
This gives the user the benefit of being able to differentiate a variable vs an object

Which is crucial to the development since it will not compile if it is not working.

- this is known as catch errors in development

TypeScript allows the code to be used as documentation since it labels the specific type of variable in the function

# Project
## Purpose
The purpose for this project is to learn how to interact TypeScript with the React rather than just a general overview of React

### State Hook w/ TypeScript
```TypeScript
const [number, setNumber] = useState(5);
const changeNumber = () => {
  setNumber( 10);
}
```
TypeScript inferred that the variable `setNumber` is of type number

```TypeScript
const [coworker, setCoworkers] = useState([
  {
  name: "Ankur", role: "swe manager",
  },
  {
    name: "Pasamba",
    role: "product owner",
  }
])

coworker.map(coworker => {
coworker.role;
})
```
Example of hard coded data

#### General data
You will initialize your types inside of an interface rather than them being stored inside of a ''`<>`'' before a state

```TypeScript
interface Foo {
  coworker:{
    name:string;
    role:string;
    email?: string;
  }[]
}
```
This interface begins by first stating what the value of the object coworker which is an array comprised of name, role, and email. Now if you want to make a variable optional in the creation of the array use must use a "`?`" before declaring the type

Now how do you integrate with the `useState()`?

You simply just call it inside the `<>` to specify which element inside the interface. **ASB**

```TypeScript
const[coworker, setCoworkers] = useState<Foo["coworker"]>([])
```
 which as you can deconstruct into a type (`<>`) then FOO array (`Foo[]`), which contains the name of the variable (`Foo["coworker"]`) then an open state

### Props example
For components to be added you with create a separate folder which is up to the programmers discretion on how to organize. According to the [crash course](https://www.youtube.com/watch?v=jrKcJxF0lAU), inside the folder you will create a `.tsx` file.

Then intialize React
```TypeScript
 import React from "react";
 ```
Then continue to the creation of your components  
