# Learning Flexbox

## Code

### Basics

```css
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: Ariel, Helvetica, sans-serif;
}

.flex-container {
    height: 400px;
    display: flex;
    flex-direction: row;
    flex-direction: row-reverse;
    flex-direction: column;
    background: #f4f4f4;
    /* main axis */
    justify-content: end; /* main axis */
    justify-content: start; /* main axis */
    justify-content: center; /* main axis */
    justify-content: space-around; /* main axis */
    justify-content: space-between; /* main axis */
    justify-content: space-evenly; /* main axis */

     /*cross axis */
    align-items: end;
    align-items: start;
    align-items: center;

    flex-wrap: wrap;

}

.item {
    flex: 1 0 100px;
    flex: 1 0 1px;
    flex: 1;
    width: 100px;
    flex-basis: 300px;
    height: 100px;
    background: #254de4;
    color: white;
    margin: 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    /*flex-grow: 1;*/

}

.item:nth-of-type(1) {
    align-self: start;
    order: 2;
    flex-grow: 10;
    flex-shrink: 1;
}

.item:nth-of-type(2) {
    align-self: center;
    order: 1;
    flex-basis: 200px;
    flex-grow: 1;
    flex-shrink: 2;
}

.item:nth-of-type(3) {
    align-self: end;
    order: 3;
    flex-grow: 1;
    flex-shrink: 3;
}
```

### Project

```css
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: "Arial Hebrew Scholar";
    font-size: 16px;
    line-height: 1.5;
    color: #333;
    background: #a1c3ff;
}

img {
    max-width: 100%;
}

h1, h2 {
    margin-bottom: 15px;
}

.container {
    max-width: 1100px;
    margin: 0 auto;
    padding: 0 30px;
}

ul {
    list-style-type: none;
}

.navbar {
    background: #3474e6;
    color: #fff;
    height: 60px;
}

.navbar .logo {
    font-size: x-large;
    font-weight: bold;
}

.navbar a {
    color: white;
    text-decoration: none;
    font-size: 18px;
    font-weight: bold;
}

.navbar a:hover {
    color: lightblue;
}

.navbar .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100%;
}

.navbar ul {
    display: flex;
}

.navbar ul li {
    margin-left: 20px;
}

.header {
    background-color: #0151cc;
    color: white;
    min-height: 400px;
    display: flex;
}

.header h1 {
    font-size: 3rem;
    font-weight: bold;
    line-height: 1.2;
}

.header img {
    max-width: 400px;
    margin: 20px;
}

.header .container {
    height: 400px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.boxes .container {
    display: flex;
    justify-content: space-between;
}

.box {
    flex: 1;
    background: #0a51cc;
    color: #fff;
    border-radius: 10px;
    margin: 20px 10px;
    box-shadow: 0 3px 5px rgba(0, 0, 0, 0.6);
    padding: 15px 20px;
}

.box i {
    margin-right: 10px;
}

@media (max-width: 768px) {
    .header .container {
        flex-direction: column;
        padding-top: 20px;
        text-align: center;
    }

    .boxes .container {
        display: block;
        text-align: center;
    }
}
```
## Credits

- [youtube | Flexbox Crash Course 2022](https://www.youtube.com/watch?v=3YW65K6LcIA&ab_channel=TraversyMedia)