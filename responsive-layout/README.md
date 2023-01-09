<br><br>
<h1 align=center><b>Responsive Layout - with HTML & CSS</b></h1>

<br>

## **HTML**
```html

<!DOCTYPE html>
<html>
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Design</title>
    <style>
        body {
            min-height: 100vh;
            background-color: #f7f7f7;
            display: grid;
            gap: 10px;
            grid-template-rows: 60px 2fr .5fr .5fr 60px;
        }
        body > *{
            border-radius: 5px;
        }
        header, footer {
            background-color: #7030A0;
        }
        main {
            background-color: #E29CE4;
        }
        aside, section {
            background-color: #CA47CD;
        }

        @media (min-width: 37.5em) {        /*   For Tablets   */
            body {
                grid-template-columns: 1fr 1fr;
                grid-template-rows: 60px 2fr 1fr 60px;
            }
            header, main, footer {
                grid-column: 1/-1;
            }
        }

        @media (min-width: 56.25em) {       /*   For Desktops   */
            body {
                grid-template-columns: 1fr 2fr 1fr;
                grid-template-rows: .5fr 1fr .2fr;
            }
            aside {
                grid-column: 1/2;
                grid-row: 2/4;
            }
            main {
                grid-column: 2/3;
                grid-row: 2/3;
            }
            footer {
                grid-row: 3;
                grid-column: 2/-1;
            }
        }
    </style>
</head>
<body>
    <header></header>
    <main></main>
    <aside></aside>
    <section></section>
    <footer></footer>
</body>
</html>
```
<br>

## **OUTPUT**

<div align=center>
<img src="preview.png" aria-hidden="true">
</div>
