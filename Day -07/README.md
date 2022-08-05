# DAY_07_TASK 

##### 1.	https://github.com/rvsp/typescript-oops/blob/master/Practice/Movie.md

**Class – Movie;**

Ans:

        class Movie {
            constructor (title, studio, rating = "PG") {
                this.title = title
                this.studio = studio
                this.rating = rating
            }
        }
        const favMovie = new Movie("Casino Royale", "Eon Productions" , "PG13")
        console.log(favMovie);



##### 2.	https://github.com/rvsp/typescript-oops/blob/master/Practice/class-circle.md

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
        console.log(a.getradius());
        console.log(a.getcolor());
        console.log(a.getarea());
        console.log(a.getcircumference());


### 3.	Write a “person” class to hold all the details.

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




### 4.	write a class to calculate uber price.

        class uberprice{
            constructor(baseprice,kilometre,tax){
                this.baseprice=baseprice;
                this.kilometre=kilometre;
                this.tax=tax;
            }
        }

        const price = new uberprice(100,10,200); 

        console.log(price);

