# Part 1: React-Assessment
 
## 1. Why does React utilize the virtual-dom?
React uses the virtual-dom in memory in order to create a dynamic web app. Otherwise,
The virtual DOM creates a virtual representation with DOM manipulation
 
## 2a How is data flowed in React? 

Data is flowed in a unidirectional way or in other words downward.

## 2b. Why is React architected this way?
Architecting it in this way ensure there is no spagetthi code. It also improves performance and efficent, easier to debug and its structed much better.
 
## 3. What is the purpose for lifting state up in React? Give an example of this
The purpose of lifting state up in React is to transfer data from one child component to its sibiling. This is done by transfering data from child1 component => to parent component => then to child2 component. A stateful parent component is necessary so that the child components can share data from the parent component. 

Ex:

parent => child1 => parent => child2
- Parent: Fruit Container
- Child1: Fruit Filter
- Child2: Fruit List

Data is passed down to the parent it is then filtered into child2 and send back to fruit container to then go down to child2 to render the fruit list

 
## 4. Why would a startup be interested in applying React-Router to a project? Explain in detail.
Using React-Router allows for much more efficent run-time on components in a React project. It also created unique url link for different pages/ components to render. React-Router is also much easier to use and when user view different components their state is saved so it makes them dyanamic.

## 5. Can browsers read JSX? Why?
No, modern browsers at this time cannot read JSX. The reason being that browsers interpret js version ES5. Instead, a complier called Babel is used to translate JSX code to be render to a browser.
 
## 6. What is the significance of keys in React? 
When mapping data, React needs us to define each item by a key value. Order is important when rendering. Otherwise, we will get an error message telling us to include keys in our map function.
 
## 7. What is the difference between Props and State?
Props: used to pass data from parent into child components

State: it's a repository of data, it holds local data of a component
 
## 8. Examine the code below: In relation to React, explain what is occurring, and why it’s significant. 
 
Babel Input: ES2015 arrow function
`[1, 2, 3].map( n => n + 1 )`
 
Babel Output: ES5 equivalent
```
[1,2,3].map(function(n) {
Return n + 1;
})
 
```
The babel input is a much more shorter way of coding the example in babel output. It is also using an anonynmous function. This is one of the reasons babel is used in react to complie what's in the input to then render this code to the browser using ES5.

## 9. Given the array of strings: names, return a new array with each name properly capitalized. Must use .map() 
```
const names = [ “james”, “joseph”, “diamond”, “gillian”]
function properNames(names) {
    name.map
}
```
