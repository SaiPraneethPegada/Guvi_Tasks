# Write a blog on Difference between HTTP1.1 vs HTTP2.

    •	HTTP2 loads faster than HTTP1.1
    
    •	HTTP2 is binary, where as HTTP1 is textual.
    
    •	HTTP2 is fully multiplexed, instead of ordered and blocking
    
    •	HTTP2 can, therefore, use one connection for parallelism
    
    •	HTTP2 uses header compression to reduce overhead
    
    •	HTTP2 allows servers to “push” responses proactively into client caches.
    
    •	HTTP2 is secured by default.
    

# Write a blog about objects and its internal representation in JavaScript. 

    •	Object: An Object is a collection of properties and methods. (Object is also a Data Type in JavaScript. 
        It can contain properties of all the other types starting from Number, String, Boolean, Arrays, and even other Objects)
   
    •	These properties are written in the form of Key-Value pair.
    
    •	There are 2 ways to access properties of the Object: using a Dot operator and using Bracket notation. {Ex: Student.name; and Student[‘name’];}
    
    •	There are 3 ways to define an object:
        o	Using an Object literal
        o	Using the New keyword
        o	Using Object Constructor.
        
    •	Using Object Literal: 
        o	Ex: var Student = {name: “Guvi”, class: 31, roll_no: 1};
        o	From the above example Student is Object.
        
    •	Using New Keyword:
            Ex: 
            var Student = new object();
            Student.name = “Guvi”;
            Student.class = 31;
            Student.roll_no = 1;
        o	Dot Operator(.) is used to write keys and assign values to it.
        
    •	Using Object Constructor: is a function which has the same name as the Object.
            Ex: 
            Function Student(name, class, roll_no){
            this.name = name;
            this.class = class;
            this.roll_no = roll_no;
            }
            var Student1 = new Student("Guvi",31,1);
