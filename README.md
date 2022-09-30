# css-workout
 By training on the css features, I make it possible to use it all the time.

> ### Normalize.css
A modern, HTML5-ready alternative to CSS resets <br>
Normalize.css makes browsers render all elements more consistently and in line with modern standards. It precisely targets only the styles that need normalizing. If you want to take a look, you can check: [Normalize.css](https://necolas.github.io/normalize.css/) <br>
So I used normalize.css to get the same output in all browsers.

> ### Using flexbox

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

> ### Using grid

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

> ### Using position

![using-position](images/using-position.png)

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

> ### Using flex & margin

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

> ### Using grid & margin

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