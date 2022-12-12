<!DOCTYPE html>
<html>
    <head>
        <style>
        *{
            padding: 0;
            margin: 0;
            box-sizing: border-box;
            font-family: 'Josefin Sans', sans-serif;
            scroll-behavior: smooth;
            list-style: none;
            text-decoration: none;
        }
        *::selection{
            background: chocolate;
            color: #FFFDD0;
        }
        body{
            color: #999999;
            background: chocolate;
        }
        header{
            position:absolute;
            top: 0;
            right: 0;
            width: 100%;
            z-index: 1000;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }
        .logo{
            color: #4b5320;
            font-weight: 600;
            font-size: 2.4rem;
        }
        .navbar a{
            color: #4b5320;
            font-size: 1.1rem;
            padding: 10px 20px;
            font-weight: 500;
        }
        .navbar a:hover{
            color: beige;
            transition: .4s;
        }
        #menu-icon{
            font-size: 2rem;
            cursor:pointer;
            display: none;
        }
        section{
            padding: 70px 17%;
        }
        .home{
            width: 100%;
            min-height: 90vh;
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            grid-gap: 1.5rem;
            align-items: center;
        }
        .home-img img{
            max-width: 100%;
            width: 600px;
            height: auto;
        }
        .home-text h1{
            font-size: 3rem;
            color: #4b5320;
        }
        .home-text h2{
            font-size: 1.5rem;
            margin: 1rem 0 2rem;
        }
        .btn{
            display: inline-block;
            padding: 10px 20px;
            background: chocolate;
            color: brown;
            border-radius: 0.5rem;
        }
        .btn:hover{
            transform: scale(1.2) translate(10px);
            transition: .4s;
        }
        .about{
            display: grid;
            grid-template-columns: repeat(2, 2fr);
            grid-gap: 1.5rem;
            align-items: center;
        }
        .about-img img{
            max-width: 100%;
            width: 480px;
            height: auto;
        }
        .about-text span{
            color: #5C4033;
            font-weight: 600;
        }
        .about-text h2{
            font-size: 2.25rem;
        }
        .about-text p{
            margin: 0.8rem 1.8rem;
            line-height: 1.7;
        }
        .heading{
            text-align: center;
        }
        .heading span{
            color: #5C4033;
            font-weight: 600;
        }
        .heading h2{
            font-size: 2rem;
        }
        .menu-container{
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, auto));
            grid-gap: 1.5rem;
            align-items: center;
        }
        .box{
            position: relative;
            margin-top: 4rem;
            height: auto;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            background: #C4BDAC;
            padding: 20px;
            border-radius: 0.5rem;
        }
        .box-img{
            width: 220px;
            height: 220px;
        }
        .box-img img{
            width: 100%;
            height: 100%;
        }
        .box h2{
            font-size: 1.3rem;
            color: #5C4033;
        }
        .box h3{
            color: #5C4033;
            font-size: 1rem;
            font-weight: 400;
            margin: 4px 0 10px;
        }
        .box span{
            font-size: 1rem;
            color: #5C4033;
            font-weight: 600;
        }
        .box .bx{
            background: #5C4033;
            position: absolute;
            right: 0;
            top: 0;
            font-size: 20px;
            padding: 7px 10px;
        }
        .heading{
            text-align: center;
        }
        .heading span{
            color: #5C4033;
            font-weight: 600;
        }
        .heading h2{
            font-size: 2rem;
        }
        .services{
            position: relative;
            margin-top: 4rem;
            height: auto;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            background: #C4BDAC;
            padding: 20px;
            border-radius: 0.5rem;
        }
        .s-box-img{
            width: 220px;
            height: 220px;
        }
        .s-box-img img{
            width: 100%;
            height: 100%;
        }
        .services h2{
            font-size: 1.3rem;
            color: #5C4033;
        }
        .services h3{
            color: #5C4033;
            font-size: 1rem;
            font-weight: 400;
            margin: 4px 0 10px;
        }
        .service-container{
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, auto));
            grid-gap: 1.5rem;
            align-items: center;
        }
        </style>

        <meta charset="utf-8"/>
        <meta name="viewport" content="width=device-width", initial-scale="1.0" />
        <title>Kuku's Bakery Cafe</title>
        <link rel="stylesheet" type="text/css" href="css/style.css" />

        <link rel="stylesheet"
        href="https://unpkg.com/boxicons@latest/css/boxicons.min.css">

    </head>
    <body style="background: beige">

        <header>
            <ul class="navbar; display: flex">
            <div style=" color: #483C32; font-weight: 600; font-size: 2.4rem;">
            <a href="#" class="logo" style="color: #483C32;font-family: 'Fredoka One', cursive;">Kuku's Bakery Cafe</a>
            </div>
            </ul>
            <div class="bx bx-menu" id="menu-icon"></div>

            <ul class="navbar">
                <div style="position:absolute; top: 0; right: 0; width: 100%; z-index: 1000; display: flex; align-items: center; justify-content: right; padding: 30px 170px;">
                <a href="#home" style="color: #483C32;  font-family: 'Josefin Sans', sans-serif; color: #4b5320;font-size: 1.1rem;padding: 10px 20px;font-weight: 500;">Home</a><br>
                <a href="#about" style="color: #483C32;  font-family: 'Josefin Sans', sans-serif; color: #4b5320;font-size: 1.1rem;padding: 10px 20px;font-weight: 500;">About Us</a><br>
                <a href="#menu" style="color: #483C32;  font-family: 'Josefin Sans', sans-serif; color: #4b5320;font-size: 1.1rem;padding: 10px 20px;font-weight: 500;">Menu</a><br>
                <a href="#services" style="color: #483C32;  font-family: 'Josefin Sans', sans-serif; color: #4b5320;font-size: 1.1rem;padding: 10px 20px;font-weight: 500;">Services</a><br>
                <a href="#products" style="color: #483C32;  font-family: 'Josefin Sans', sans-serif; color: #4b5320;font-size: 1.1rem;padding: 10px 20px;font-weight: 500;">Products</a><br>
                <a href="#contact" style="color: #483C32;  font-family: 'Josefin Sans', sans-serif; color: #4b5320;font-size: 1.1rem;padding: 10px 20px;font-weight: 500;">Contact Us</a>
                </div>
            </ul>
        </header>

        <!--------home start-------->
        <section class="home" id="home">
            <div class="home-text">
                <h1 style="font-family: 'Yuji Syuku', serif;">Kuku's Bakery Cafe</h1>
                <h2>Gather around, friends.<br>Let's talk about coffee, pastries and<br>pasta all over again</h2>
                <a href="#" class="btn">Today's Coffee</a>
            </div>

            <div class="home-img">
                <img src="img/cookies.jpg">
            </div>
        </section>

        <!--------about start-------->
        <section class="about" id="about">
            <div class="about-img">
                <img src="img/about.jpg">
            </div>

            <div class="about-text">
                <span>About Us</span>
                <h2>Today's good mood<br>is sponsored by Coffee</h2>
                <h3>there are many chuchuchu we are located at chhuchcuch</h3>
                <a href="#" class="btn">Today's Coffee</a>
            </div>
        </section>

        <!--------menu start-------->
        <section class="menu" id="menu">
            <div class="heading">
                <span>Food Menu</span>
                <h2>Fresh taste and great price</h2>
            </div>

            <div class="menu-container">
                <div class="box">
                    <div class="box-img">
                        <img src="img/crinkles.jpg" width="150" height="150">
                    </div>
                    <h2>Choco Crinkles</h2>
                    <h3>Super Yummy</h3>
                    <span>35 pesos</span>
                    <i class='bx bx-cart-alt'></i>
                </div>


                <div class="box">
                    <div class="box-img">
                        <img src="img/brown.jpg" width="150" height="150">
                    </div>
                    <h2>Triple Choco Brownies</h2>
                    <h3>Super Yummy</h3>
                    <span>70 pesos</span>
                    <i class='bx bx-cart-alt'></i>
                </div>


                <div class="box">
                    <div class="box-img">
                        <img src="img/coo.jpg" width="150" height="150">
                    </div>
                    <h2>Choco Cookies</h2>
                    <h3>Super Yummy</h3>
                    <span>35 pesos</span>
                    <i class='bx bx-cart-alt'></i>
                </div>

                <div class="box">
                    <div class="box-img">
                        <img src="img/alfred.jpg" width="150" height="150">
                    </div>
                    <h2>Alfredo Pasta</h2>
                    <h3>Super Yummy</h3>
                    <span>35 pesos</span>
                    <i class='bx bx-cart-alt'></i>
                </div>

                <div class="box">
                    <div class="box-img">
                        <img src="img/coo.jpg" width="150" height="150">
                    </div>
                    <h2>Choco Crinkles</h2>
                    <h3>Super Yummy</h3>
                    <span>35 pesos</span>
                    <i class='bx bx-cart-alt'></i>
                </div>

                <div class="box">
                    <div class="box-img">
                        <img src="img/coo.jpg" width="150" height="150">
                    </div>
                    <h2>Choco Crinkles</h2>
                    <h3>Super Yummy</h3>
                    <span>35 pesos</span>
                    <i class='bx bx-cart-alt'></i>
                </div>
            </div>
        </section>

        <!--------service start-------->
        <section class="services" id="services">
            <div class="heading">
                <span>Services</span>
                <h2>We provide the best quality food and drinks</h2>
            </div>

            <div class="service-container">
                <div class="s-box">
                    <img src="img/panda" width="250" height="150">
                    <h3>Order</h3>
                    <p>food panda grab lalamovehafhsuidisugv</p>
                </div>

                <div class="s-box">
                    <img src="img/grab.jpg" width="250" height="150">
                    <h3>Order</h3>
                    <p>Grab Food</p>
                </div>
            </div>
        </section>
    </body>
</html>

