# Project Responsive Web Design using Bootstrap
## Date:

## AIM:
To design a responsive website for a Pharmaceutical Company using Bootstrap.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
<html>
    <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title> Product Page </title>
        <style type="text/css">
            * {
                margin: 0;
                padding: 0;
                font-family: Arial, Helvetica, sans-serif;
            }
            .banner {
                width: 100%;
                height: 100vh;
                background-image: linear-gradient(rgba(0,0,0,0.75),rgba(0,0,0,0.75)),url(back.jpg);
                background-size: cover;
                background-position: center;
            }
            .navbar {
                width: 85%;
                margin: auto;
                padding: 35px 0;
                display: flex;
                align-items: center;
                justify-content: space-between;
            }
            .bg-product {
                border: 1px;
                padding: 10px;
                color: white;
                background-color:  #00d5ff;
                border-radius: 30px;
            }
            .logo {
                color:  #fb0b0b;
                font-size: 40px;
                font-weight: 700;
                letter-spacing: 3px;
            }
            span {
                color: white;
            }
            form {
                width: 300px;
                height: 40px;
                display: flex;
                background: rgba(255,255, 255, 0.1);
                padding: 1px 1px;
                font-size: 15px;
                border-radius: 10px;
                backdrop-filter: blur(4px) saturate(180%);
            }
            form input {
                background: transparent;
                flex: 1;
                border: 0;
                outline: none;
                padding: 12px 20px;
                font-size: 15px;
                color: white;
            } 
            ::placeholder {
                color: white;
            }
            form button {
                border: 0;
                outline: none;
                padding: 5px 20px;
                color: white;
                border-radius: 10px;
                background:  #00d5ff;
                cursor: pointer;
            }
            .navbar li {
                list-style: none;
                display: inline-block;
                margin: 0 20px;
                position: relative;
            }
            .navbar li a {
                text-decoration: none;
                color: white;
                text-transform: uppercase;
            }
            .navbar li:hover {
                border: 1px;
                padding: 10px;
                color: white;
                background-color:  #00d5ff;
                transition: 0.5s; 
                cursor: pointer;
                border-radius: 30px;
            }
            .container {
                background: transparent;
                padding: 10px 5%;
                padding-bottom: 100px;
            }
            .container .box-container {
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(170px, 1fr));
                gap: 100px;
            }
            .container .box-container .box {
                color: white;
                box-shadow: 0 5px 10px rgba(0,0,0,.2);
                border-radius: 20px;
                background: transparent;
                border: 1px solid white;
                padding: 30px 20px;
            }
            .container .box-container .box img {
                height: 70px;
                border-radius: 20px;
            }
            .container .box-container .box h3 {
                color:  #00d5ff;
                font-size: large;
                padding: 20px 0;
            }
            .container .box-container .box p {
                color: white;
                font-size: small;
                line-height: 1.5;
            }
            footer {
                background-color: #94f60b;
                margin-top: auto;
                font-size: 20px;
            }
        </style>
    </head>
<body>
    <div class="banner">
        <br>
        <div class="navbar">
            <h1 class="logo">C<span>ode</span>W<span>ars</span></h1>
            <ul>
                <li><a href="http://127.0.0.1:8000/static/home.html"> Home </a></li>
                <li><a href="http://127.0.0.1:8000/static/product.html" class="bg-product"> Products </a></li>
                <li><a href="http://127.0.0.1:8000/static/people.html"> People </a></li>
                <li><a href="http://127.0.0.1:8000/static/contact.html"> Contact </a></li>
            </ul>
            <form action="" method="get">
                <input type="text" placeholder="Enter to Search">
                <button type="submit"> Search </button>
            </form>
        </div>
        <div class="container">
            <div class="box-container">
                <div class="box">
                    <img src="c++.png" alt="">
                    <h3> C++ </h3>
                    <p>  C++ is a cross-platform language that can be used to create high-performance applications.</p>
                </div>
                <div class="box">
                    <img src="java.jpeg" alt="">
                    <h3> JAVASCRIPT </h3>
                    <p> JavaScript is a lightweight, cross-platform, single-threaded, and interpreted compiled programming language. I </p>
                </div>
                <div class="box">
                    <img src="php.jpeg" alt="">
                    <h3> PHP</h3>
                    <p> PHP is a server side scripting language that is embedded in HTML. </p>
                </div>
                <div class="box">
                    <img src="python.jpeg" alt="">
                    <h3> PYTHON </h3>
                    <p> Python is a popular programming language. It was created by Guido van Rossum, and released in 1991. </p>
                </div>
                <div class="box">
                    <img src="sql.jpeg" alt="">
                    <h3> SQL </h3>
                    <p> SQL is a standard language for accessing and manipulating databases. </p>
                </div>
                
                <!-- <div class="box">
                    <img src="c ash.jpg" alt="">
                    <h3> C# </h3>
                    <p> C# is used to develop web apps, desktop apps, mobile apps, games and much more.

                    </p>
                </div>
                <div class="box">
                    <img src="typescript.png" alt="">
                    <h3>TYPESCRIPT</h3>
                    <p> ypeScript is a syntactic superset of JavaScript which adds static typing. </p>
                </div>
                <div class="box">
                    <img src="f.png" alt="">
                    <h3> F# </h3>
                    <p> F# is an Open-source programming language with a lot of features.</p>
                </div>
                <div class="box">
                    <img src="swift.png" alt="">
                    <h3> SWIFT</h3>
                    <p> Swift, developed by Apple, is the go-to language for iOS and macOS app development.  </p>
                </div>
                <div class="box">
                    <img src="go.jpg" alt="">
                    <h3> GO </h3>
                    <p> Go, also known as Golang, has gained attention for its efficiency, simplicity, and strong support for concurrent programming </p>
                </div> -->
            </div>
        </div>
    </div>
    <footer>
        <center> Designed and Developed by PAVITHRAN S(212223240113) </center>
    </footer>
</body>
</html>
```


## OUTPUT:
![alt text](output.png)


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
