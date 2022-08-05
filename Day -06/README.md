# Day_06_Task

## Part-1: Find the culprits and nail them — debugging javascript

### 1.	Fix the below to alert Guvi geek

        let admin=9, fname=10.5; 
        fname = "Guvi";
        lname = "geek"
        admin = `${fname} ${lname}`;
        alert(admin); //Prints  “Guvi Geek”

### 2.	Fix the below to alert hello Guvi geek

        let fname=10.5; 
        fname = "Guvi";
        lname = "geek"
        let fullName = `${fname} ${lname}`;
        alert( `hello ${fullName}` );  //Prints  “hello Guvi geek”

### 3.	Fix the below to alert sum of two numbers

        let a = parseInt(prompt("First number"));
        let b = parseInt(prompt("Second number"));
        alert(a + b);

### 4.	If you run the below script you will get “Code is Blasted” Explain Why the Code is blasted and how to diffuse it and get “Diffused”.
  var a = "2" > "12";
  //Don't touch below this
  if (a) {
    console.log("Code is Blasted")
  }
  else
  {
    console.log("Diffused") 
  }
	
	
        Explanation: If we run the above snippet we get Code is Blasted because in the condition the variables provided are strings, they are not integers to satisfy the condition of greater than (>).

        To get Diffused:
        var a = 2 > 12;
        //Don't touch below this
        if (a) {
        console.log("Code is Blasted")
        }
        else
        {
        console.log("Diffused") 
        }


### 5.	How to get the success in console.

        let a = parseInt(prompt("Enter a number?"));
        //Don't modify any code below this
        if (a) {
         console.log( 'OMG it works for any number inc 0' );
        }
        else
        {
         console.log( "Success" );
        }

### 6.	How to get the correct score in console.

        let value = parseInt(prompt('How many runs you scored in this ball'));
        if (value === 4) {
              console.log("You hit a Four");
        } else if (value === 6) {
              console.log("You hit a Six");
        } else {
              console.log(value);
        }
				
				
### 7.	Fix the code to welcome the boss

        let message;
        let lock = '';
        //Dont change any code below this 
        if (null || lock || undefined )
        {
        message = "Go away";
        }
        else
        {
        message = "welcome";
        }
        console.log(message);

### 8.	Change the code to print

  3
  2
  1
  
        let i = 3;
        let diff=3;
        while (i--)
        {
        console.log(diff--);
        }

### 9.	Change the code to print 1 to 10 in 4 lines

        let n = 10;
        for (let i=1; i<11; i++){
           console.log(i);
        }


### 10.	Change the code to print even numbers

        for (let num = 2; num <= 20; num += 2) {
          console.log(num)
        }
				
----


## PART-2: Find the culprits and nail them — debugging javascript loops

### 11.	Change the code to print all the gifts

        let gifts = ["teddy bear", "drone", "doll"];
        for (let i = 0; i < gifts.length; i++) {
          console.log(`Wrapped ${gifts[i]} and added a bow!`);
        }


### 12.	Write a code to print the numbers in the array

  Output: 1234567891011

        var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
        var new_string = "";

        for (var i = 0; i < 11; i++) {
          new_string += numsArr[i] 
        }
        console.log(new_string);


### 13.	Write a code to print from last to first with spaces (Make sure there is no space after the last element 1)

  Output: 11 10 9 8 7 6 5 4 3 2 1

        var new_string = "";

        for (var i = 11; i > 0; i-- ) {
         new_string += [i] + " " 
        }
        console.log(new_string.trim());



### 14.	Write a code to replace the array value — If the number is even, replace it with ‘even’.
Output:[ 1, “even”, 3, “even”, 5, “even”, 7, “even”, 9, “even”, … ]

        var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
        for (var i = 0; i <=10; i++) {
            if(numsArr[i] %2 === 0 ){
            numsArr[i] ="even";
        }
        }
        console.log(numsArr);



### 15.	Write a code to replace the array value — If the index is even, replace it with ‘even’.
Output: [ “even”, 2, “even”, 4, “even”, 6, “even”, 8, “even”, 10, … ]

        var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
          for (var i = 0; i <=10; i++) {
          if(numsArr[i] %2 === 1 ){
          numsArr[i] = "even";
              }
        }
        console.log(numsArr);


### 16.	Write a code to add all the numbers in the array
Output: 66.

        var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
        let sum= 0;
        for (var i = 0; i<11; i++) {
        sum += numsArr[i];
        }
        console.log(sum);

### 17.	Write a code to add the even numbers only
Output: 30

        var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
        var sum=0;
        for (var i = 0; i<11; i++) {
        if(numsArr[i]%2===0){
        sum += numsArr[i];
        }
        }
        console.log(sum);

### 18.	Write a code to add the even numbers and subract the odd numbers
Output: 94

        var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
        var sum=100;
        for (var i = 0; i <=10; i++) {
          if(numsArr[i]%2!==1){
          sum += numsArr[i]
          } 
         else{
          sum -= numsArr[i]
          }
        }
        console.log(sum);


### 19.	 Write a code to print inner arrays
Output: 	Array(5) [ 1, 2, 3, 4, 5 ]
					Array(6) [ 6, 7, 8, 9, 10, 11 ]

        var numsArr = [[1, 2, 3, 4, 5],[ 6, 7, 8, 9, 10, 11]];
        for (var i = 0; i < numsArr.length; i++) {
         console.log( numsArr[i])
        }

### 20.	 Write a code to print elements in the inner arrays
Output: 1234567891011

        var numsArr = [[1, 2, 3, 4, 5],[ 6, 7, 8, 9, 10, 11]];
        var str_all="";
        for (var i = 0; i < numsArr.length; i++) {
         var inner_array = numsArr[i];
         for(var j = 0 ; j < inner_array.length;j++ ) {
             str_all = inner_array[j]
             console.log(str_all);
            }}
						
----

## PART-3: Find the culprits and nail them — debugging javascript

### 21.	 Fix the code to get the largest of three.

        const aa = (f,s,t) => {
         if(f>s &&f>t){
         console.log(f)}
         else if(s>f && s>t){
         console.log(s)}
         else{
         console.log(t)}
        }
        aa(6,2,3);


### 22.	Fix the code to Sum of the digits present in the number

        let n = 1234;
        let a = n.toString();
        let b = a.split("");

        function add(b)
        {
        let sum = 0;
        for(var i=0;i<b.length;i++){
         sum+=parseInt(b[i])
         }
         return parseInt(sum);
        }
        console.log(add(b));



### 23.	Fix the code to Sum of all numbers using IIFE function

        const arr = [9,8,5,6,4,3,2,1];
        let sum = 0;

        let total = (function() {
         for (var i = 0; i < arr.length; i++){
         sum += arr[i];
         }
         return sum;
        })
        console.log(total(sum));

### 24.	Fix the code to gen Title caps.

        var arr = ["guvi", "geek", "zen", "fullstack"];
        var ano = function(arro) {
         for (var i = 0; i < arr.length; i++) {
         console.log(arr[i][0].toUpperCase() + arr[i].substr(1));
         }
        }
        ano();


### 25.	Fix the code to sum the number in that array

        const num = [10, 20, 30, 40,50,60,70,80,90,100] 
        let sum = (a, b) => a + b
        sum = num.reduce(sum)
        console.log(sum);


### 26.	print all odd numbers in an array using IIFE function

        var arr = [1, 2, 3, 5, 7, 79, 7, 2, 6, 9, 4];
        (function() {
         for (var i = 0; i < arr.length; i++) {
         if (arr[i] % 2 === 1) {
         console.log(arr[i]);
         }}
        })();


### 27.	Fix the code to reverse.

        (function(str){
         str1 = str.split("").reverse().join("");
         console.log(str1); 
        })("abcd")

### 28.	Sum of odd numbers in an array

        var as=[12,34,5,6,2,56,6,2,1];

        var s=as.reduce(function(a,c){
         if(c%2 != 0)
         {
         return a+c;
         }
         return a;},0);
        console.log(s);



### 29.	Fix the code to give the below output:
Expected Output:
[
{firstName: “Vasanth”, lastName: “Raja”, age: 24, role: “JSWizard”},
{firstName: “Sri”, lastName: “Devi”, age: 28, role: “Coder”}
]
		
        var array = [
        [
          ["firstname", "vasanth"],
          ["lastname", "Raje"],
          ["age", 24],
          ["role", "JSWizard"],
        ],
        [
          ["firstname", "Sri"],
          ["lastname", "Devi"],
          ["age", 28],
          ["role", "Coder"],
        ],
      ];

      var final = [];
      let i = 0;
      while (i< array.length) {
        var outer_remove = array.shift();
        var new_object = {};

        while (outer_remove.length != 0 ) {
          var inner_remove = outer_remove.shift();
          var key = inner_remove[0];
          var value = inner_remove[1];
          new_object[key] = value;
        }

        final.push(new_object);
      }
      console.log(final)
  			


### 30.	Fix the code to remove duplicates.

        var res = function(arr){
        var newArr = [];
        for(var i=0; i < arr.length; i++)
        {
         if(newArr.indexOf(arr[i]) == -1) 
        {
             newArr.push(arr[i]);
         }
        }
        console.log(newArr)
        }
        res(['guvi','geek','guvi','duplicate','geeK', 'guvi']);



