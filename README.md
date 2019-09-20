<html>
    <head>
        <style>
        body {
            background-color: rgb(238, 237, 237);
        }
        h1 {
            font-family: 'Courier New', Courier, Monospace;
            font-size: 43px;
            text-align: center;
            font-style: initial;
            color:rgb(223, 175, 175);
            font-weight: lighter;
        }
        input {
            text-align: left;
            cursor: text;
            font-size: 16px;
            border-radius: 10px 10px 10px 10px;
            border-style: hidden;
            border-width: 1px;
            box-shadow: 2px 2px 3px #494848;
            background-color: #f3e7e7;
            font-weight: lighter;
            padding: 15px;
        }
        span {
            text-align: left;
            cursor: pointer;
            font-size: 16px;
            border-radius: 10px 10px 10px 10px;
            border-style: hidden;
            border-width: 1px;
            box-shadow: 2px 2px 3px #494848;
            background-color: #f3e7e7;
            color: #6b6868;
            font-weight: lighter;
            padding: 15px;
        }
        ul li {
            margin: 0;
            padding: 0;
            position: relative;
            cursor: pointer;
            
        }
        footer {
            margin-top: 450px;
            height: 100px;
            padding: 10px;
            width: 100%;
            font-size: 12px;
            text-align: center;
            color: #494848;
        }
        </style>

        <body>
            <script src="https://kit.fontawesome.com/88379ff677.js"></script>
            <div id='app'>
                <section class='todoApp'>
                    <header class='header'>
                    <h1>todos</h1>                    
                    <input id='new-todo' class='new-todo' type='text' placeholder='Enter a new task...'>
                    <span onclick="newElement()" class="addBtn">Add</span>
                    </header>
                </section>
                <ul id="myUL">
                    <li class="checked">Visit granny</li>
                    <li>Meet friends</li>
                    <li>Buy products</li>
                    <li>Do ACA homework</li>
                    <li>Read a book</li>
                </ul>
            </div>
            <footer>
                <div>
                    <p>&#169 2019 Arevik Harutyunyan<p>
                    <i class="fas fa-anchor"> </i>
                </div>
            </footer>
        </body>
        
        <script>
        
        </script>
    </head>
</html>
