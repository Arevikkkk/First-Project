<html>
    <head>
        <style>
        body {
            background-color: rgb(238, 237, 237);
        }
        h1 {
            height: 5%;
            font-family: 'Courier New', Courier, Monospace;
            font-size: 90px;
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
            width: 45%;
        }
        span {
            text-align: center;
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
            position: relative;
            cursor: pointer;
            padding: 15px;
            width: 400%;
            font-size: 16px;
            border-radius: 10px 10px 10px 10px;
            border-style: hidden;
            border-width: 1px;
            box-shadow: 2px 2px 3px #494848;
            background-color: #f8f2f2;
            font-weight: lighter;
        }
        ul li:hover {
            background-color: rgb(255, 255, 255);
        }
        footer {
            position: fixed;
            bottom: 0;
            height: 80px;
            width: 100%;
            font-size: 12px;
            text-align: center;
            color: #494848;
        }
        li i {
            position: absolute;
            right: 0;
            top: 0;
            padding: 16px;
            color: #494848;
        }
        li i:hover {
            color: #d15252;
        }
        .flex-container {
            display: flex;
        }
        </style>

        <body>
            <script src="https://kit.fontawesome.com/88379ff677.js"></script>
            <div id='app'>
                <section class='todoApp'>
                    <header class='header'>
                    <h1>todos</h1>                    
                    <input id='new-todo' type='text' placeholder='Enter a new task...'>
                    <span onclick='newTodo()' class='addBtn'>Add</span>
                    </header>
                </section>
                <div class='flex-container'>
                <ul id='UL'>
                    <li class="checked">Visit granny <i class="fas fa-trash-alt"></i></li>
                    <li>Meet friends <i class="fas fa-trash-alt"></i></li>
                    <li>Buy products <i class="fas fa-trash-alt"></i></li>
                    <li>Do ACA homework <i class="fas fa-trash-alt"></i></li>
                    <li>Read a book <i class="fas fa-trash-alt"></i></li>
                </ul>
                </div>
            </div>

            <footer>
                <div>
                    <p>&#169 2019 Arevik Harutyunyan<p>
                    <i class="fas fa-anchor"> </i>
                </div>
            </footer>
        </body>
        
        <script>
            const close = document.getElementsByClassName("fas fa-trash-alt");
            for (let i = 0; i < close.length; i++) {
                close[i].onclick = function() {
                    let div = this.parentElement;
                    div.style.display = 'none';
                }
            }

            function newTodo() {
                let li = document.createElement('li');
                let inputValue = document.getElementById('new-todo').value;
                let txt = document.createTextNode(inputValue);
                li.appendChild(txt);
                if (inputValue === '') {
                    alert('Please, write something.');
                } else {
                    document.getElementById('UL').appendChild(li);
                }
                document.getElementById('new-todo').value = '';

                let i = document.createElement('i')
                i.className = "fas fa-trash-alt";
                li.appendChild(i);

                const close = document.getElementsByClassName("fas fa-trash-alt");
                for (let i = 0; i < close.length; i++) {
                    close[i].onclick = function() {
                    let div = this.parentElement;
                    div.style.display = 'none';
                    }
                }
            }

        </script>
    </head>
</html>
