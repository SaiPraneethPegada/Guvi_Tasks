# Day_08_Task

###  Solving problems using array functions on rest countries data.

a.	Get all the countries from Asia continent /region using Filter function

```javascript
<script>
        var request = new XMLHttpRequest();
        request.open('GET', 'https://raw.githubusercontent.com/rvsp/restcountries-json-data/master/res-countries.json');
        request.send();
        request.onload = function () {
            var data = JSON.parse(request.response);
            let countries = data.filter((e) => {
                if (e.region === "Asia") {
                    return d.name;
                }
            })
            console.log(countries);
        }
</script>
```

b.	Get all the countries with a population of less than 2 lakhs using Filter function

```javascript
<script>
        var request = new XMLHttpRequest();
        request.open('GET', 'https://raw.githubusercontent.com/rvsp/restcountries-json-data/master/res-countries.json');
        request.send();
        request.onload = function () {
            var data = JSON.parse(request.response);
            let countries = data.filter((e) => {
                if (e.population < 200000) {
                    return d.name;
                }
            })
            console.log(countries);
        }
</script>
```

c.	Print the following details name, capital, flag using forEach function

```javascript
<script>
        var request = new XMLHttpRequest();
        request.open('GET', 'https://raw.githubusercontent.com/rvsp/restcountries-json-data/master/res-countries.json');
        request.send();
        request.onload = function () {
            var data = JSON.parse(request.response);
            data.forEach(e => {
                console.log(e.name, e.capital, e.flag)
            });
        }
</script>
```

d.	Print the total population of countries using reduce function

```javascript
<script>
        var request = new XMLHttpRequest();
        request.open('GET', 'https://raw.githubusercontent.com/rvsp/restcountries-json-data/master/res-countries.json');
        request.send();
        request.onload = function () {
            var data = JSON.parse(request.response);
            //console.log(data);
            const population = data.reduce((acc, ele) => {
                return acc + ele.population;
            }, 0);
            console.log(population)
        }
</script>
```

e.	Print the country which uses US Dollars as currency.

```javascript
<script>
        var request = new XMLHttpRequest();
        request.open('GET', 'https://raw.githubusercontent.com/rvsp/restcountries-json-data/master/res-countries.json');
        request.send();
        request.onload = function () {
            var data = JSON.parse(request.response);
            var cur = [];
            for (i = 0; i < data.length; i++) {
                if (data[i].currencies[0].code === "USD") {
                    console.log("Country -", data[i].name, "==>", `"${data[i].currencies[0].code}"`)
                }
            }
        }
</script>
```
