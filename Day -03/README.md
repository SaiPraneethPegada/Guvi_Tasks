# Day_03_Task

###  1. For the given JSON iterate over all for loops (for, for in, for of, forEach)

      var person = [{"fname":"John", "lname":"Doe", "age":25} , {"fname":"Joseph", "lname":"Doe", "age":28}];
      
        //for loop:
          for (var i=0; i<person.length; i++) {
          console.log(person[i]);
          }

        //for-in loop:
          for (var i in person) {
          console.log(person[i]);
          }

        //for of loop:
          for (const key of person) {
          console.log(key);
          }

        //forEach loop:
          person.forEach(function(key) {
          console.log(key.fname, key.lname);
          });


###  2.	Create your own resume data in JSON format

        {
          "basic": {
            "name": "Sai Praneeth Pegada",
            "label": "Full Stack Developer",
            "email": "saipraneethpegada@gmail.com",
            "phone": "+91 7386000126",
            "location": {
              "address": "Q.no-53B, Pranahitha Colony, Mandamarri",
              "postalCode": "504231",
              "city": "Mancherial",
              "state": "Telangana",
              "country": "India"
            },
            "profiles": [
              {
                "network": "Instagram",
                "username": "Praneeth_p.s.p",
                "url": "https://www.instagram.com/praneeth_p.s.p/"
              }
            ]
          },
          "work": [
            {
              "name": "Cyient",
              "position": "Reliability Engineer",
              "Location": "Bengaluru",
              "url": "https://www.cyient.com/aerospace-defense/aerospace-aftermarket-solutions",
              "startDate": "2021-06-23",
              "endDate": "2022-08-24",
              "summary": "Description…",
              "highlights": [""]
            }
          ],
          "education": [
            {
              "institution": "Telangana State Aviation Academy",
              "url": "http://tsaahyd.in/",
              "area": "Aircraft Maintenance Engineer",
              "studyType": "BSc",
              "startDate": "2017-07-15",
              "endDate": "2021-03-25",
              "score": "82%",
              "courses": ["Aircraft Maintenance Engineering"]
            }
          ],
          "skills": [
            {
              "name": "Web Development",
              "level": "Beginner",
              "keywords": ["HTML", "CSS", "JavaScript"]
            }
          ],
          "languages": [
            {
              "language": "English",
              "fluency": "Intermediate"
            }
          ],
          "interests": [
            {
              "name1": "Video Games",
              "name2": "Reading Books"
            }
          ]
        }    
