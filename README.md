    <!DOCTYPE html>
    <html lang="en">
    <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;600;700;800&display=swap');

        * {
            margin: 0;
            padding: 0;
        }

        body {
            line-height: 1;
            font-size: 100%;
            font-family: 'Open Sans', sans-serif;
            color: #5a5a5a;
        }

        #container {
            width: 980px;
            margin: 0 auto;
            box-shadow: 0 0 1em #cccccc;
        }

        header {
            padding: 20px;
        }
        header h1 {
            margin: 20px 10px;
            color: #b5b5b5;
        }

        nav {
            display: block;
            background-color: #1f5faa;
        }
        nav a {
            padding: 15px 30px;
            display: inline-block;
            color: #ffffff;
            font-size: 14px;
            text-decoration: none;
            font-weight: bold;
        }
        nav a.active,
        nav a:hover {
            background-color: #2b83ea;
        }

        #hero {
            background-color: #e4e4e5;
            padding: 50px 20px;
            margin-bottom: 20px;
        }
        #hero h1 {
            margin-bottom: 20px;
            font-size: 35px;
        }
        #hero p {
            margin-bottom: 20px;
            font-size: 18px;
            line-height: 25px;
        }

        #wrapper {
            margin: 0;
        }
        #main {
            float: left;
            width: 640px;
            padding: 20px;
        }
        #sidebar {
            float: left;
            width: 260px;
            padding: 20px;
        }

        .widget-box {
            border: 1px solid #eee;
            margin-bottom: 20px;
        }
        .widget-box .title {
            padding: 10px 16px;
            background-color: #428bca;
            color: #fff;
        }
        .widget-box ul {
            list-style-type: none;
        }
        .widget-box li {
            border-bottom: 1px solid #eee;
        }
        .widget-box li a {
            padding: 10px 16px;
            color: #333;
            display: block;
            text-decoration: none;
        }
        .widget-box li:hover a {
            background-color: #eee;
        }
        .widget-box p {
            padding: 15px;
            line-height: 25px;
        }

        footer {
            clear: both;
            background-color: #1d1d1d;
            padding: 20px;
            color: #eee;
        }

        .box {
            display: block;
            float: left;
            width: 33.333%;
            box-sizing: border-box;
            padding: 0 10px;
            text-align: center;
        }
        .box h3 {
            margin: 15px 0;
        }
        .box p {
            line-height: 20px;
            font-size: 14px;
            margin-bottom: 15px;
        }
        .image-circle {
            border-radius: 50%;
        }

        .row {
            margin: 0 -10px;
            box-sizing: border-box;
        }
        .row:after {
            content: '';
            display: table;
            clear: both;
        }

        .divider {
            border: 0;
            border-top: 1px solid #eeeeee;
            margin: 40px 0;
        }

        /* Entry */
        .entry {
            margin: 15px 0;
        }
        .entry h2 {
            margin-bottom: 20px;
        }
        .entry p {
            line-height: 25px;
        }
        .entry img {
            float: left;
            border-radius: 5px;
            margin-right: 15px;
        }
        .entry .right-img {
            float: right;
        }
    </style>
    </head>
    <body>
    <div id="container">
        <header>
            <h1>Layout Sederhana</h1>
        </header>
        
        <nav>
            <a href="home.html" class="active">Home</a>
            <a href="artikel.html">Artikel</a>
            <a href="about.html">About</a>
            <a href="kontak.html">Kontak</a>
        </nav>

        <section id="hero">
            <h1>Hello World!</h1>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
            <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
        </section>

        <section id="wrapper">
            <section id="main">
                <div class="row">
                    <div class="box">
                        <img src="https://dummyimage.com/120/db7d25/fff.png" alt="" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                    <div class="box">
                        <img src="https://dummyimage.com/120/3e73e6/fff.png" alt="" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                    <div class="box">
                        <img src="https://dummyimage.com/120/71e6d4/fff.png" alt="" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                </div>

                <hr class="divider" />

                <article class="entry">
                    <h2>First featurette heading.</h2>
                    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
                </article>

                <hr class="divider" />

                <article class="entry">
                    <h2>Second featurette heading.</h2>
                    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" class="right-img">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
                </article>
            </section>

            <aside id="sidebar">
                <div class="widget-box">
                    <h3 class="title">Widget Header</h3>
                    <ul>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                        <li><a href="#">Widget Link</a></li>
                    </ul>
                </div>
                <div class="widget-box">
                    <h3 class="title">Widget Text</h3>
                    <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
                </div>
            </aside>
        </section>

        <footer>
            <p>&copy; 2024- Universitas Pelita Bangsa</p>
        </footer>
    </div>
    </body>
    </html>
![Cuplikan layar 2024-11-09 203035](https://github.com/user-attachments/assets/eb649ac0-b0b4-4d9d-b358-450ab4ebb62b)



