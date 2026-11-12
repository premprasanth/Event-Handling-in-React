# React Lab Exercise 4: Event Handling in React
## Name: PREM PRASANTH J
## Roll no: 2305001028
## Department: CSE

## AIM
### To understand and implement event handling in React using events such as onClick, onChange, and onSubmit. 

## PROGRAM
### App.jsx  
### i) onClick Event function
```py
App() {   function handleClick() {     alert("Button was clicked!"); 
  }   return ( 
    <div> 
      <h1>React Event Handling</h1> 
      <button onClick={handleClick}> 
        Click Me 
      </button> 
    </div> 
  ); 
} export default App;
```
 
### ii) onClick with State
```py
import { useState } from "react"; function App() {   const [count, setCount] = useState(0);   function handleClick() {     setCount(count + 1); 
  }   return ( 
    <div> 
      <h1>Click Counter</h1> 
      <h2>Button clicked: {count} times</h2> 
      <button onClick={handleClick}> 
        Click Me 
      </button> 
    </div> 
  ); 
} export default App; 
 ```
### iii) onChange Event 
```py
import { useState } from "react"; function App() {   const [name, setName] = useState("");   function handleChange(event) {     setName(event.target.value); 
  }   return ( 
    <div> 
      <h1>Student Name</h1> 
      <input 
        type="text" 
        placeholder="Enter your name"         onChange={handleChange} 
      /> 
      <h2>Hello, {name}</h2> 
    </div> 
  ); 
} export default App; 
```
## OUTPUT
<img width="1125" height="401" alt="image" src="https://github.com/user-attachments/assets/d3db34a0-13a6-4846-bd47-e8b26a93f530" />
<img width="1125" height="413" alt="image" src="https://github.com/user-attachments/assets/82e76a76-6ffd-42eb-bc57-f9342489ed05" />
<img width="2368" height="880" alt="image" src="https://github.com/user-attachments/assets/88b45936-6c44-44c3-b057-79d24ce1ab4c" />

##  RESULT
### Thus, React event handling was successfully implemented using the onClick and onChange events. The application responded to button clicks, maintained a click counter using useState, and displayed the student's name dynamically based on user input.
