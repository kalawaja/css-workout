# css-workout
 By training on the css features, I make it possible to use it all the time.

> ### Normalize.css
A modern, HTML5-ready alternative to CSS resets <br>
Normalize.css makes browsers render all elements more consistently and in line with modern standards. It precisely targets only the styles that need normalizing. If you want to take a look, you can check: [Normalize.css](https://necolas.github.io/normalize.css/) <br>
So I used normalize.css to get the same output in all browsers.

> ## 5 Ways to Center a Div in CSS  

> ### 1. Using flexbox

![using-flexbox](images/using-flexbox.png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Using flexbox</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="normalize.css">
</head>
<body>
    <div class="parent">
        <div class="parent"></div>
        <div class="parent"></div>
    </div>
</body>
</html>
```

```css
#styles.css

/*Using flexbox*/

.parent {
    width: 200px;
    height: 200px;
    border: 1px solid;
    display: flex;
    justify-content: center;
    align-items: center;
}
```

> ### 2. Using grid

![using-grid](images/using-grid.png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8">
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Using grid</title>
   <link rel="stylesheet" href="styles.css">
   <link rel="stylesheet" href="normalize.css">
</head>
<body>
   <div class="parent">
       <div class="child"></div>
       <div class="child"></div>
   </div>
</body>
</html>
```

```css
#styles.css

/*Using grid*/

.parent {
    width: 200px;
    height: 200px;
    border: 1px solid;
}

.child {
    width: 50px;
    height: 50px;
    border: 1px solid;
    display: grid;
    place-content: center;
}
```

> ### 3. Using position

![using-position](images/using-position.png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8">
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Using position</title>
   <link rel="stylesheet" href="styles.css">
   <link rel="stylesheet" href="normalize.css">
</head>
<body>
   <div class="parent">
       <div class="child"></div>
       <div class="child"></div>
   </div>
</body>
</html>
```

```css
#styles.css

/*Using position*/

.parent {
    width: 200px;
    height: 200px;
    border: 1px solid;
    position: relative;
}

.child {
    width: 50px;
    height: 50px;
    border: 1px solid;
    position: absolute;
    top: 50%;
    left:50%;
    transform: translate(-50%, -50%);
}
```

> ### 4. Using flex & margin

![using-flex-margin](images/using-flex-margin.png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8">
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Using flex & margin</title>
   <link rel="stylesheet" href="styles.css">
   <link rel="stylesheet" href="normalize.css">
</head>
<body>
   <div class="parent">
       <div class="child"></div>
       <div class="child"></div>
   </div>
</body>
</html>
```

```css
#styles.css

/*Using flex & margin*/

.parent {
    width: 200px;
    height: 200px;
    border: 1px solid;
    display: flex;
}

.child {
    width: 50px;
    height: 50px;
    border: 1px solid;
    margin: auto;
}
```

> ### 5. Using grid & margin

![using-grid-margin](images/using-grid-margin.png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8">
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Using grid & margin</title>
   <link rel="stylesheet" href="styles.css">
   <link rel="stylesheet" href="normalize.css">
</head>
<body>
   <div class="parent">
       <div class="child"></div>
       <div class="child"></div>
   </div>
</body>
</html>
```

```css
#styles.css

/*Using grid & margin*/

.parent {
    width: 200px;
    height: 200px;
    border: 1px solid;
    display: grid;
}

.child {
    width: 50px;
    height: 50px;
    border: 1px solid;
    margin: auto;
}
```
---

> ## CSS Combinator Selectors

> ### 1. Descendant Selector

![descendant-selector](images/descendant-selector.png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8">
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Descendant Selector</title>
   <link rel="stylesheet" href="styles.css">
   <link rel="stylesheet" href="normalize.css">
</head>
<body>
   <div class="container">
        <h1>Lorem</h1>
        <h2>Ipsum</h2>
        <h3>Dolor</h3>
        <h4>Sit</h4>
        <h5>Amet</h5>
        <h6>Consectetur</h6>
   </div>
</body>
</html>
```

```css
#styles.css

/*Descendant Selector*/

.container h3 {
    border: 1px solid black;
    max-width: 50px;
    text-align: center;
    background-color: bisque;
}
```

> ### 2. Adjacent Sibling Selector

![adjacent-sibling-selector](images/adjacent-sibling-selector.png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8">
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Adjacent Sibling Selector</title>
   <link rel="stylesheet" href="styles.css">
   <link rel="stylesheet" href="normalize.css">
</head>
<body>
   <div class="container">
        <h3>Lorem</h3>
        <h3>Ipsum</h3>
    </div>
    <h3>Dolor</h3>
    <h3>Sit</h3>
    <h3>Amet</h3>
    <h3>Consectetur</h3>
</body>
</html>
```

```css
#styles.css

/*Adjacent Sibling Selector*/

div + h3 {
    border: 1px solid black;
    max-width: 50px;
    text-align: center;
    background-color: thistle;
}
```

> ### 3. Child Selector

![child-selector](images/child-selector.png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8">
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Child Selector</title>
   <link rel="stylesheet" href="styles.css">
   <link rel="stylesheet" href="normalize.css">
</head>
<body>
   <div class="container">
        <p>Lorem</p>
        <p>Ipsum</p>
    </div>
    <p>Dolor</p>
    <p>Sit</p>
    <p>Amet</p>
    <p>Consectetur</p>
</body>
</html>
```

```css
#styles.css

/*Child Selector*/

div > p {
    border: 1px solid black;
    max-width: 60px;
    text-align: center;
    background-color: powderblue;
}
```

> ### 4. General Sibling Selector

![genereal-sibling-selector](images/genereal-sibling-selector.png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8">
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Genereal Sibling Selector</title>
   <link rel="stylesheet" href="styles.css">
   <link rel="stylesheet" href="normalize.css">
</head>
<body>
   <div>
        <p>Lorem</p>
        <p>Ipsum</p>
    </div>
    <p>Dolor</p>
    <p>Sit</p>
    <p>Amet</p>
    <p>Consectetur</p>
</body>
</html>
```

```css
#styles.css

/*General Sibling Selector*/

div ~ p {
    border: 1px solid black;
    max-width: 100px;
    text-align: center;
    background-color: lightgreen;
}
```

> ### 5. Chained Class Selector

![chained-class-selector](images/chained-class-selector.png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8">
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Chained Class Selector</title>
   <link rel="stylesheet" href="styles.css">
   <link rel="stylesheet" href="normalize.css">
</head>
<body>
   <div class="container1 select2">
        <p>Lorem</p>
        <p>Ipsum</p>
    </div>
    <div class="container1 select3">
        <p>Dolor</p>
        <p>Sit</p>
        <p>Amet</p>
        <p>Consectetur</p>
    </div>
    <div class="container1 select2">
        <p>Adipisicing</p>
        <p>Elit.</p>
    </div>
</body>
</html>
```

```css
#styles.css

/*Chained Class Selector*/

.container1.select2 {
    border: 1px solid black;
    max-width: 100px;
    text-align: center;
    background-color: royalblue;
}
```

> ## CSS :nth-child Selectors  

> ### 1. :last-child

![last-child](images/last-child.png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS :last-child Selector</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="/css-workout/normalize.css">
</head>
<body>
    <div class="parent">
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
    </div>
</body>
</html>
```

```css
#styles.css

/*CSS:last-child Selector*/

.parent {
    background: #f1f1f1;
    border: 1px solid black;
    width: 100%;
    padding: 10px 0;
    margin: 10px 0;
    display: flex;
    flex-wrap: nowrap;
    justify-content: space-around;
}

.child {
    border: 1px solid black;
    border-radius: 50%;
    width: 20px;
    height: 20px;
}

.child:last-child {
    background: red;
}
```

> ### 2. :nth-child(2)

![nth-child(2)](images/nth-child(2).png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS :nth-child(2) Selector</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="/css-workout/normalize.css">
</head>
<body>
    <div class="parent">
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
    </div>
</body>
</html>
```

```css
#styles.css

/*CSS:nth-child(2) Selector*/

.parent {
    background: #f1f1f1;
    border: 1px solid black;
    width: 100%;
    padding: 10px 0;
    margin: 10px 0;
    display: flex;
    flex-wrap: nowrap;
    justify-content: space-around;
}

.child {
    border: 1px solid black;
    border-radius: 50%;
    width: 20px;
    height: 20px;
}

.child:nth-child(2) {
    background: red;
}
```

> ### 3. :nth-child(even)

![nth-child(even)](images/nth-child(even).png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS :nth-child(even) Selector</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="/css-workout/normalize.css">
</head>
<body>
    <div class="parent">
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
    </div>
</body>
</html>
```

```css
#styles.css

/*CSS:nth-child(even) Selector*/

.parent {
    background: #f1f1f1;
    border: 1px solid black;
    width: 100%;
    padding: 10px 0;
    margin: 10px 0;
    display: flex;
    flex-wrap: nowrap;
    justify-content: space-around;
}

.child {
    border: 1px solid black;
    border-radius: 50%;
    width: 20px;
    height: 20px;
}

.child:nth-child(even) {
    background: red;
}
```

> ### 4. :nth-child(n+3)

![nth-child(n+3)](images/nth-child(n+3).png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS :nth-child(n+3) Selector</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="/css-workout/normalize.css">
</head>
<body>
    <div class="parent">
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
    </div>
</body>
</html>
```

```css
#styles.css

/*CSS:nth-child(n+3) Selector*/

/* for (n=0, n++) */

.parent {
    background: #f1f1f1;
    border: 1px solid black;
    width: 100%;
    padding: 10px 0;
    margin: 10px 0;
    display: flex;
    flex-wrap: nowrap;
    justify-content: space-around;
}

.child {
    border: 1px solid black;
    border-radius: 50%;
    width: 20px;
    height: 20px;
}

.child:nth-child(n+3) {
    background: red;
}
```

> ### 5. :nth-child(3n+1)

![nth-child(3n+1)](images/nth-child(3n+1).png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS :nth-child(3n+1) Selector</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="/css-workout/normalize.css">
</head>
<body>
    <div class="parent">
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
    </div>
</body>
</html>
```

```css
#styles.css

/*CSS:nth-child(3n+1) Selector*/

/* for (n=0, n++) */

.parent {
    background: #f1f1f1;
    border: 1px solid black;
    width: 100%;
    padding: 10px 0;
    margin: 10px 0;
    display: flex;
    flex-wrap: nowrap;
    justify-content: space-around;
}

.child {
    border: 1px solid black;
    border-radius: 50%;
    width: 20px;
    height: 20px;
}

.child:nth-child(3n+1) {
    background: red;
}
```

> ### 6. :nth-last-child(2)

![nth-last-child(2)](images/nth-last-child(2).png)

```html
#index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS :nth-last-child(2) Selector</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="/css-workout/normalize.css">
</head>
<body>
    <div class="parent">
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
        <div class="child"></div>
    </div>
</body>
</html>
```

```css
#styles.css

/*CSS:nth-last-child(2) Selector*/

.parent {
    background: #f1f1f1;
    border: 1px solid black;
    width: 100%;
    padding: 10px 0;
    margin: 10px 0;
    display: flex;
    flex-wrap: nowrap;
    justify-content: space-around;
}

.child {
    border: 1px solid black;
    border-radius: 50%;
    width: 20px;
    height: 20px;
}

.child:nth-last-child(2) {
    background: red;
}
```