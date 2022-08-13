# DAY_07_TASK 

##### 1.	https://github.com/rvsp/typescript-oops/blob/master/Practice/Movie.md

**Class – Movie;**

Ans:

```javascript
class Movie {
    constructor (title, studio, rating = "PG") {
        this.title = title
        this.studio = studio
        this.rating = rating
    }
}
const favMovie = new Movie("Casino Royale", "Eon Productions" , "PG13")
console.log(favMovie);

// Output : Movie { title: 'Casino Royale', studio: 'Eon Productions', rating: 'PG13' }
```


##### 2.	https://github.com/rvsp/typescript-oops/blob/master/Practice/class-circle.md

```javascript
let pi = 3.1412;
class circle {
  constructor(radius, color) {
    this.radius = radius;
    this.color = color;
  }
  getradius() {
    return this.radius;
  }
  getcolor() {
    return this.color;
  }
  getarea() {
    return pi * this.radius * this.radius;
  }
  getcircumference() {
    return 2 * pi * this.radius;
  }
}
let a = new circle(1.0, "red");
console.log(a.getradius());         // Prints : 1
console.log(a.getcolor());          // Prints : red
console.log(a.getarea());           // Prints : 3.1412
console.log(a.getcircumference());  // Prints : 6.2824
```

### 3.	Write a “person” class to hold all the details.

```javascript
class Person {
    constructor (firstName, lastName, DOB, address, jobTitle, yearsOfExperience) {
        this.firstName = firstName
        this.lastName = lastName
        this.DOB = DOB
        this.address = address
        this.jobTitle = jobTitle
        this.yearsOfExperience = yearsOfExperience
    }
}

const details = new Person("Sai Praneeth", "Pegada" , "13 Nov" , "H.no-53B Pranahitha Colony" , "Full stack", 0)

console.log(details);       

/* Output : Person {
  firstName: 'Sai Praneeth',
  lastName: 'Pegada',
  DOB: '13 Nov',
  address: 'H.no-53B Pranahitha Colony',
  jobTitle: 'Full stack',
  yearsOfExperience: 0 } */
```



### 4.	write a class to calculate uber price.

```javascript
class uberprice{
    constructor(baseprice,kilometre,tax){
        this.baseprice=baseprice;
        this.kilometre=kilometre;
        this.tax=tax;
    }
}

const price = new uberprice(100,10,200); 

console.log(price);         // Output : uberprice { baseprice: 100, kilometre: 10, tax: 200 }
```
