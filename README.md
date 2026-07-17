Practical 1
1.Environment Setup and JavaScript Basics 

a. Install Node.js and Visual Studio Code, and verify installation. 
node -v
npm -v

b. Create a simple Node.js file and run it using the terminal. 
CODE:-
console.log(“Hello welcome to Mern Practical”);
console.log(“Priti Yadav”);

c. Write a Node.js script demonstrating basic JavaScript commands(console log, variables, and arithmetic operations). 
CODE:- 
let num1 = 10; 
let num2 = 20; 
console.log("First number:",num1); 
console.log("Second number:",num2);
console.log("Addition:",num1+num2); 
console.log("Subtraction:",num1-num2); 
console.log("Multiplication:",num1*num2); 
console.log("Division:",num1/num2); 
console.log("Priti Yadav"); 

d. Create and run a simple program using variables and functions. CODE:- 
let num1 = 10; 
let num2 = 20;  
function add(num1,num2){ 
 return num1+num2; 
} 
function multiply(num1,num2){ 
 return num1*num2; 
} 
console.log("First number:",num1); 
console.log("Second number:",num2); 
console.log("Addition:",add(num1,num2)); 
console.log("Multiplication:",multiply(num1,num2)); 
console.log("Priti Yadav"); 

e. Demonstrate use of operators and control statements in JavaScript CODE:- 
let a=20; 
let b=10; 
//comparison operator 
console.log("\nComparison Operators"); 
console.log("a>b:",a>b); 
console.log("a<b:",a<b); 
console.log("a==b:",a==b); 
console.log("a!=b:",a!=b);
//If-Else Statement 
console.log("\nIf-Else Statement"); 
if(a>b){ 
 console.log("a is greater than b"); 
} 
else{ 
 console.log("b is greater than or equal to a") 
} 
//switch statement 
console.log("\nswitch statement"); 
let day=2; 
switch(day){ 
 case 1: 
 console.log("Monday"); 
 break; 
 case 2: 
 console.log("Tuesday"); 
 break; 
 case 3: 
 console.log("Wednesday"); 
 break; 
 default: 
 console.log("Invalid day"); 
} 
console.log("Priti Yadav"); 

f. Write programs using loops and template literals. CODE:- 
let number=5; 
console.log(`multiplication table of ${number}`); 
for(let i = 1; i <=10; i++) 
{ 
 console.log(`${number} x ${i} = ${number*i}`); 
  
} 
console.log("Priti Yadav");

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Practical 2

2. Core JavaScript Concepts for MERN 
a. Create functions and call them with parameters. 
CODE:- 
For calculateSalary 
function calculateSalary(name,basicSalary){ 
 let bonus=5000; 
 let totalSalary=basicSalary+bonus; 
 console.log("Employee Name:",name); 
 console.log("Basic salary:",basicSalary); 
 console.log("Bonus:",bonus); 
 console.log("total salary:",totalSalary); 
} 
calculateSalary("Priti",50000); 
console.log("Priti Yadav T054"); 

For Generating bill with 18% GST. 
CODE:- 
function genBill(Product,Quantity,Price){ 
 let total=Quantity*Price; 
 let bill=total+(total*0.18); 
 console.log("Product:",Product); 
 console.log("Quantity:",Quantity); 
 console.log("Price per Item:",Price); 
 console.log("total Bill:",bill); 
} 
genBill("Fridge",2,50000); 
console.log("Priti Yadav T054");

b. Work with arrays and objects in JavaScript. 
CODE:- 
//Array 
let fruits=["Mongo","Banana","Apple","Cherry"]; 
//Object 
let student={ 
 name:"Priti", 
 age:19, 
 city:"Kolkata" 
}; 
console.log("Fruits:",fruits); 
console.log("Second Fruits:",fruits[1]); 
console.log("Student Name:",student.name); 
console.log("Student Age:",student.age); 
console.log("Student city:",student.city); 
console.log("Priti Yadav T054"); 

c. Demonstrate use of arrow functions. 
CODE:- 
let add=(a,b)=>{ 
 return a+b 
}; 
let sub=(a,b)=>{ 
 return a-b 
}; 
let mul=(a,b)=>{ 
 return a*b 
}; 
let div=(a,b)=>{ 
 return a/b 
}; 
console.log("Addition:",add(10,10)); 
console.log("Subtraction:",(22,19)); 
console.log("Multiplication:",(10,10)); 
console.log("Division:",(15,5)); 
console.log("Priti Yadav T054");

d. Write a program using array methods (map, filter, reduce). CODE:- 
let numbers=[10,20,30,40,50]; 
//map() 
let doubled=numbers.map(num =>num*2); 
//filter 
let greater25=numbers.filter(num=>num>25); 
//reduce 
let total=numbers.reduce((sum,num)=>sum+num,0); 
console.log("Original Array:",numbers); 
console.log("Map:",doubled); 
console.log("Filter:",greater25); 
console.log("Reduce:",total); 
console.log("Priti Yadav T054"); 

e. Create a program that manipulates objects and displays output. CODE:- 
//Creating an object 
let student={ 
 rollNo:54, 
 name:"Priti", 
 marks:83 
}; 
console.log("Original Object"); 
console.log(student); 
//2.Accessing Properties 
console.log("\nAccessing Properties:"); 
console.log("Name:",student.name); 
console.log("Marks:",student.marks); 
//updating properties 
student.marks=90; 
console.log("\nAfter Updating Marks:"); 
console.log(student); 
//Adding a new Property 
student.marks=90; 
console.log("\nAfter updating marks:"); 
console.log(student);
//Deleting a Property 
delete student.rollNo; 
console.log("\nAfter Deleting Roll Number:"); 
console.log(student); 
console.log("Priti Yadav T054"); 

f. Implement a small JavaScript program combining functions, arrays,and objects. CODE:- 
//Array of object 
let students=[ 
 { 
 rollNo:54, 
 name:"Priti", 
 marks:83 
}, 
{ 
 rollNo:32, 
 name:"khushiii", 
 marks:90 
}, 
{ 
 rollNo:7, 
 name:"subuu", 
 marks:92 
}, 
{ 
 rollNo:31, 
 name:"ishuu", 
 marks:98 
} 
]; 
//function display 
function display(s) 
{
console.log("Student details"); 
console.log("----------------"); 
for(let stud of s) 
{ 
 console.log(`Roll No:${stud.rollNo}`); 
 console.log(`Name:${stud.name}`); 
 console.log(`Marks:${stud.marks}`); 
 console.log("----------------"); 
} 
} 
//function call 
display(students); 
console.log("Priti Yadav T054"); 

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Practical3

3.React Introduction and JSX 
a. Create a React application using Vite/CRA and display “Welcome to MERN Stack Development”. CODE:- 
function App() 
{ 
return( 
<div> 
<h1>Welcome to Mern Stack Development</h1> 
<h3>Hello Priti T054</h3> 
</div> 
);} 
export default App 

b. Display dynamic data using JSX. 
i) React program to display employee details (name, department, salary) using JSX. 
CODE:- 
function App() 
{ 
const emp ="Priti"; 
const dept="IT"; 
const sal =50000; 
return( 
<div> 
<h1>Employee Details</h1> 
<p>Name:{emp}</p> 
<p>Department:{dept}</p> 
<p>Salary:${sal}</p> 
<h3> Priti Yadav T054</h3> 
</div> 
); 
} 
export default App 

ii)React program to display student attendance details using variables and JSX CODE:- 
function App(){ 
const studentName="Priti Yadav"; 
const totalClasses=60; 
const attendedClasses=55; 
const attendance=(attendedClasses/totalClasses)*100; 
return( 
<div> 
<h1> Attendance Dashboard</h1> 
<hr/> 
<p>Name:{studentName}</p> 
<p>Total Classes:{totalClasses}</p> 
<p>Classes Attended:{attendedClasses}</p> 
<p>Attendance:{attendance.toFixed(2)}%</p> 
<h3> 
Status:{attendance>=75?"Eligible for Exam":"Not Eligible"} 
</h3> 
<h3> Priti Yadav T054</h3> 
</div> );} 
export default App 

c. Declare variables and write a function to calculate the sum of two numbers and display the result. CODE:- 
function App(){ 
const maths=85; 
const sci=90; 
function calculate(marks1,marks2){return marks1+marks2}; 
return( 
<div> 
<h1>Student Marks</h1> 
<hr /> 
<p>Mathematical Marks:{maths}</p> 
<p>Science Marks:{sci}</p> 
<hr /> 
<h3>Total Marks:{calculate(maths,sci)}</h3> 
<h3> Priti Yadav T054</h3> 
</div> 
);} 
export default App 

d. Apply basic CSS styling to a React component CODE:- 
App.css 
.container { 
width:700px; 
margin: 50px auto; 
padding: 20px; 
border: 2px solid black; 
border-radius: 10px; 
padding: 5px 10px; 
border-radius: 5px; 
background-color: whitesmoke; 
text-align: center;} 
h1{ 
color: darkblue;} 
p{ 
font-size: 18px; 
color: black;} 
button{ 
background-color: green; 
color: white; 
border: none; 
padding: 10 px 20 px; 
font-size:16px; 
border-radius: 5px; 
cursor: pointer;} 
button:hover{ 
background-color: darkgreen;} 
App.jsx 
import "./App.css"; 
function App(){ 
return( 
<div className="container"> 
<h1>Student Dashboard</h1> 
<hr/> 
<p>Name:Priti Yadav</p> 
<p>Roll Number:T054</p> 
<p>Course:BSCIT</p> 
<p>Semester:III</p> 
<button>View Result</button> 
</div>);} 
export default App; 

e. Create a simple functional component and render it in App.js. CODE:- 
Student.jsx 
function Student() { 
return ( 
<div> 
<h2>Stdeunt Component</h2> 
<p> Name: Priti Yadav</p> 
<p>Course : BSCIT </p> 
<p>Semster : III</p> 
</div>
);} 
export default Student; 
App.jsx 
import Student from "./components/Student"; 
function App() { 
return ( 
<div> 
<h1>This is functional component practical</h1> 
<hr /> 
<Student /> 
</div> 
);} 
export default App; 

f. Create a React component that displays the current date and time dynamically using JavaScript. CODE:- 
function App(){ 
//create a Date object 
const currentDate=new Date(); 
return( 
<div> 
<h1>Current Date and Time</h1> 
<hr /> 
<p>Date:{currentDate.toLocaleDateString()}</p> 
<p>Time:{currentDate.toLocaleTimeString()}</p> 
<h3> Priti Yadav T054</h3> 
</div> ); 
} 
export default App 

Student Details and Result Management System CODE:- 
Header.jsx 
function Header() { 
return ( 
<div> 
<h1>Student Information System</h1> 
<hr /> 
</div> 
);} 
export default Header; 
Student.jsx 
function Student() { 
return ( 
<div> 
<h2>Student Details</h2> 
<p>Name : Priti Yadav</p> 
<p>Course : B.Sc.IT</p> 
<p>Semester :III</p> 
</div> 
);} 
export default Student; 
Attendance.jsx 
function Attendance() { 
const tc = 60; 
const p = 55; 
const per = (p / tc) * 100; 
return ( 
<div> 
<h2>Attendance</h2> 
<p>Total Classes : {tc}</p> 
<p>Present : {p}</p> 
<p>Attendance : {per.toFixed(2)}%</p> 
</div> 
);} 
export default Attendance; 
Result.jsx 
function Result() { 
const java = 90; 
const python = 95; 
const react = 93; 
const total = java + python + react; 
const percentage = (total / 300) * 100; 
return ( 
<div> 
<h2>Result</h2> 
<p>Total Marks : {total}</p> 
<p>Percentage : {percentage.toFixed(2)}%</p> <p>Grade : A+</p> 
</div> 
);} 
export default Result; 
Footer.jsx 
function Footer() { 
return ( 
<div> 
<hr /> 
<p>© 2026 Sheth L. U. J. & Sir M. V. College</p>
</div> 
);} 
export default Footer; 
App.jsx 
import Header from "./components/Header"; 
import Student from "./components/Student"; 
import Attendance from "./components/Attendance"; 
import Result from "./components/Result";  
import Footer from "./components/Footer"; 
function App()  
{ 
return( 
<div> 
<Header /> 
<Student /> 
<hr /> 
<Attendance /> 
<hr /> 
<Result /> 
<Footer /> 
</div> 
); 
} 
export default App; 
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Practical 4

4.React Components, Props, and State 
a. Create multiple components and render them on a single page. 
CODE:- 
Header.jsx 
function Header() { 
 return ( 
 <div className="header"> 
 <h3> M. V. L U. College Placement Dashboard</h3> 
 </div> 
 );} 
export default Header; 
Student.jsx 
function Student() { 
 return ( 
 <div className="card"> 
 <h2>Student Profile</h2> 
 <p>Name: Priti Yadav</p> 
 <p>Course: Bachelor of Technology</p> 
 <p>CGPA: 8.45</p> 
 <p>Attendance: 88%</p> 
 </div> 
 );} 
export default Student; 
Eligibility.jsx 
function Eligibility() { 
 return ( 
 <div className="card"> 
 <h2>Placement Eligibility</h2> 
 <p>Minimum CGPA Required: 7</p> 
 <p>Minimum Attendance: 75%</p> 
 <p>Status: Eligible</p> 
 </div> 
 );} 
export default Eligibility; 
Placementstatus.jsx 
function Placementstatus() { 
 return ( 
 <div className="card"> 
 <h2>Placement Statistics</h2> 
 <p>Total Students: 60</p> 
 <p>Placed Students: 45</p> 
 <p>Remaining Students: 15</p> 
 <p>Placement Percentage: 75%</p>
 </div> 
 );} 
export default Placementstatus; 
Companyoffer.jsx 
function Companyoffer() { 
 return ( 
 <div className="card"> 
 <h2>Company Offers</h2> 
 <p>Company: TCS</p> 
 <p>Role: Software Developer</p> 
 <p>CTC: ₹4.5 LPA</p> 
 <p>Bonus: ₹50,000</p> 
 <p>Total Package: ₹5,00,000</p> 
 </div> 
 );} 
export default Companyoffer; 
Skillprogress.jsx 
function Skillprogress() { 
 return ( 
 <div className="card"> 
 <h2>Skill Progress</h2> 
 <p>Total Skills: 10</p> 
 <p>Completed Skills: 8</p> 
 <p>Pending Skills: 2</p> 
 <p>Progress: 80%</p> 
 </div> 
 );} 
export default Skillprogress; 
Attendance.jsx 
function Attendance() { 
 const tc = 60; 
 const p = 55; 
 const per = (p / tc) * 100; 
 return ( 
 <div> 
 <h2>Attendance</h2> 
 <p>Total Classes : {tc}</p> 
 <p>Present : {p}</p> 
 <p>Attendance : {per.toFixed(2)}%</p>  </div> 
 );} 
export default Attendance; 
Result.jsx 
function Result() { 
 const java = 90; 
 const python = 95; 
 const react = 93; 
 const total = java + python + react; 
 const percentage = (total / 300) * 100;  return ( 
 <div> 
 <h2>Result</h2> 
 <p>Total Marks : {total}</p> 
 <p>Percentage : {percentage.toFixed(2)}%</p>  <p>Grade : A+</p> 
 </div> 
 );} 
export default Result;
Footer.jsx 
function Footer() { 
 return ( 
 <div className="footer"> 
 <p>© 2026 M. V. L U. Placement Cell</p>  </div> 
 );} 
export default Footer; 
App.jsx 
import Header from "./components/Header"; 
import Student from "./components/Student"; 
import Eligibility from "./components/Eligibility"; import Placementstatus from "./components/Placementstatus"; import Companyoffer from "./components/Companyoffer"; import Skillprogress from "./components/Skillprogress"; import Footer from "./components/Footer"; 
import "./App.css"; 
function App() { 
 return ( 
 <div className="container"> 
 <Header /> 
 <Student /> 
 <Eligibility /> 
 <Placementstatus /> 
 <Companyoffer /> 
 <Skillprogress /> 
 <Footer /> 
 </div> 
 );} 
export default App; 
App.css 
body { 
 font-family: Arial; 
 background-color: #f4f4f4;} 
.container { 
 width: 80%; 
 margin: auto; 
 text-align: center;} 
.header { 
 background-color: white; 
 padding: 20px; 
 font-size: 24px; 
 border-bottom: 2px solid gray; 
} 
.card { 
 background-color: white; 
 margin: 20px 0; 
 padding: 15px; 
 border-top: 2px solid #ccc; 
} 
.card h2 { 
 color: green; 
} 
.footer { 
 margin-top: 20px; 
 padding: 10px; 
 border-top: 2px solid gray; 
}
