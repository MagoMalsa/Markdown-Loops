
# Loops

JavaScript loops are used to **repeatedly run a block of code** - until a certain condition is met.
There are several options to run a block of code, including:   
-**While**   
-**Do-while**   
-**For**  
-**For-In**  
-**For-Of**  


## While Loop

var sum = 0;  
var number = 1;  
**while** (number <= 5) {  
  sum = sum + number;
  number++;  
}  
alert("Sum = " + sum);  

#### The condition is first evaluated. If true, the block of statements following the while statement is executed. 

*Output/Process	:*  
*(If 1 is smaller or equal to 5 then perform the following code.)*  
*(1+2=3, 3+3= 6, 6+4=10, sum=10+5)*  

## Do-While Loop

var sum = 0;\
var number = 1;\
**do** {  
   sum += number;  
   number++;  
} **while** (number <= 10);   
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
1-**Initializer** (var i = 1;)  
2-**Test Condition** (i <= 50;)  
3-**Updater** (i++)


## For-In Loop

var student = { name:"Bill", age: 25, degree: "Masters" };  
**for** (var item **in** student) {  
   alert(student[item]);  
}


#### A For-In Loop iterates through the properties of an object (and executes the loop's body once for each enumerable property of the object.)

*Output/Process:*  
*("Bill", then 25, then "Masters")*  


## For-Of Loop

const array = ['a', 'b', 'c', 'd'];  
for (const item of array) {  
	console.log(item)  
}  
*Output/Process:* a, b, c, d.


#### The For-of statement creates a loop that iterates over iterable objects.


## Break

var sum = 0;  
for (var i = 1; i <= 10000; i++) {  
   sum += i;  
   if (i === 50) {  
       break;  
   }  
}  
alert("Sum = " + sum); &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;      

#### The "number++;" statement won't be executed when the loop is entered for the 50th time.

*Output/Process:*  
*(Sum = 1275 instead of 50005000 because of the Break statement.)*  

## Continue

for (var i = 1; i <= 10; i++)  
{  
   if ((i % 2) != 0) {  
      continue;  
   }  
   alert(i);          
}  


#### A Continue statement in a loop stops the execution of the current iteration and goes back to the beginning of the loop to begin the next iteration.  

