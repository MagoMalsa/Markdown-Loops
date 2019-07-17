
# Loops

JavaScript loops are used to **repeatedly run a block of code** - until a certain condition is met.
There are several options to run a block of code, including:   
-**While**   
-**Do-while**   
-**For**  
-**For-in**  


## While Loop

var sum = 0;  
var number = 1;  
**while** (number <= 5) {  &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp;*// (If 1 is smaller or equal to 5 then perform the following code.)*  
  sum = sum + number;    &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp; *//  0+1=1 (sum + number = sum), 1+2=3, 3+3= 6, 6+4=10, sum=10+5*  
  number++;        &nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*// telkens +1*  
}\
alert("Sum = " + sum); &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*// -- | "Sum = 15"*

#### The condition is first evaluated. If true, the block of statements following the while statement is executed. 


## Do-While Loop

var sum = 0;\
var number = 1;\
**do** {  
   sum += number;  
   number++;  
} **while** (number <= 10);  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *// 0+1=1, 1+2=3, 3+3=6, 6+4=10, 10+5=15, 15+6=21, 21+7=28, 28+8=36, 36+9=45, 45+10= 55*  
alert("Sum = " + sum);


#### The Do-While loop is executed **at least once** whereas the while loop may not execute at all.


## For Loop

var sum = 0;  
**for** (var i = 1; i <= 5; i++) {  
   sum = sum + i;  	
}
alert("Sum = " + sum);	


#### In a For-Loop the following is called an iteration statement => (var i = 1; i <= 50; i++) 
It consists of 3 parts:   
1-Initializer **(var i = 1;)**  
2-Test Condition **(i <= 50;)**  
3-Updater **(i++)**


## For-In Loop

var student = { name:"Bill", age: 25, degree: "Masters" };  
**for** (var item **in** student) {  
   alert(student[item]);    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // => "Bill", then 25, then "Masters"  
}


#### A For-In Loop iterates through the properties of an object (and executes the loop's body once for each enumerable property of the object.)

## Break

var sum = 0;
for (var i = 1; i <= 10000; i++) {
   sum += i;
   if (i === 50) {
       break;  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  // Sum = 1275 instead of 50005000 because of **Break** statement.
   }
}
alert("Sum = " + sum); &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;      // => Sum = 1275 


#### The "number++;" statement won't be executed when the loop is entered for the 50th time.


## Continue 


#### 

