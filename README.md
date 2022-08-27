<!DOCTYPE html>
<html lang="en">
<head>
    <body></body>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <!-- font awesome cdn link  -->
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"> 
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700&display=swap');

        :root{
            --main-color:#289be3;
        }

        *{
            font-family: 'Roboto', sans-serif;
            margin:0; padding:0;
            box-sizing: border-box;
            outline: none; border:none;
            text-decoration: none;
            text-transform: capitalize;
            transition: all .2s linear;
            line-height: 1.5;
        }
        *{
    margin: 0;
    padding: 0;
    font-family: sans-serif;
}

.hero{
    position: relative;
    width: 100%;
    height: 100vh;
    background: #eff4fd;
    position: relative;
}

nav{
    display: flex;
    width: 84%;
    margin: auto;
    padding: 20px 0;
    align-items: center;
    justify-content: space-between;
}

.logo{
    width: 100px;
    cursor: pointer;
}

nav ul li {
    display: inline-block;
    list-style: none;
    margin: 10px 20px;
}

nav ul li a{
    text-decoration: none;
    color: rgb(175, 127, 127);
    font-weight: bold;
}

nav ul li a:hover{
    color: red;
}

.detel{
    margin-left: 8%;
    margin-top: 15%;
}

.detel h1{
    font-size: 50px;
    color: #212121;
    margin-bottom: 20px;
}

span{
    color: orange;
    
}

.detel p{
    color: #555;
    line-height: 22px;
}

.detel a{
    background: #212121;
    padding: 10px 18px;
    text-decoration: none;
    font-weight: bold;
    color: #fff;
    display: inline-block;
    margin: 30px 0;
    border-radius: 5px;
}

.images{
    width: 45%;
    height: 80%;
    position: absolute;
    bottom: 0;
    right: 100px;
}

.images img{
    height: 100%;
    position: absolute;
    left: 50%;
    bottom: 0;
    transform: translateX(-50%);
    transition: bottom 1s, left 1s;
}

.images:hover .shape{
    bottom: 40px;
}

.images:hover .girl{
    left: 45%;
}

.social{
    margin-left: 8%;
    margin-top: 100px;
}

.social a{
    font-size: 30px;
    color: #212121;
    margin-right: 20px;
}

.social a:hover{
    color: orange;
}
        html{
            font-size: 62.5%;
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        body{
            background: #fcfce8;
            padding-left: 30rem;
        }

        section{
            padding:1rem 5%;
            min-height: 100vh;
        }

        .heading{
            font-size: 4rem;
            padding-bottom: 1rem;
            color:#111;
            text-transform: uppercase;
        }

        .heading span{
            color:var(--main-color);
            text-transform: uppercase;
        }

        .btn{
            display: inline-block;
            margin-top: 1rem;
            padding:.8rem 3rem;
            background:var(--main-color);
            color:#fff;
            cursor: pointer;
            font-size: 1.7rem;
        }

        .btn:hover{
            background:rgb(4, 4, 4);
            letter-spacing: .2rem;
        }

        header{
            position: fixed;
            top:0; left:0; bottom:0;
            background:#222;
            display: flex;
            align-items: center;
            justify-content: space-between;
            z-index: 1000;
            flex-flow: column;
            padding:8rem 2rem;
            width:30rem;
            text-align: center;
        }

        header .logo{
            text-transform: uppercase;
            color:#fff;
            font-size: 3rem;
            font-weight: bolder;
        }

        header .logo span{
            text-transform: uppercase;
            color:var(--main-color);
        }

        header .navbar a{
            display: block;
            font-size: 2rem;
            color:#fff;
            margin:2rem 0;
        }

        header .navbar a:hover{
            letter-spacing: .2rem;
            color:var(--main-color);
        }

        header .follow a{
            font-size: 2.5rem;
            color:#fff;
            margin:0 .7rem;
        }

        header .follow a:hover{
            color:var(--main-color);
        }

        #menu-bars{
            position: fixed;
            top:1rem; right: 1rem;
            z-index: 10000;
            background:var(--main-color);
            color:#fff;
            border-radius: .5rem;
            padding:1rem 1.5rem;
            font-size: 3rem;
            cursor:pointer;
            display: none;
        }

        .cursor-1{
            position: absolute;
            top:0; left:0;
            height:1rem; width:1rem;
            background: var(--main-color);
            pointer-events: none;
            transform: translate(-50%, -50%);
            border-radius: 50%;
            z-index: 10000;
        }

        .cursor-1.active{
            height:7rem;
            width:7rem;
            opacity: .3;
        }

        .cursor-2{
            position: absolute;
            top:0; left:0;
            height:4rem; width:4rem;
            border:.1rem solid var(--main-color);
            pointer-events: none;
            transform: translate(-50%, -50%);
            border-radius: 50%;
            z-index: 10000;
            transition: .3s linear;
        }

        .cursor-2.active{
            display: none;
        }

        .home{
            display: flex;
            align-items: center;
            flex-wrap: wrap;
            gap:1.5rem;
            background-image: url(https://img.freepik.com/free-photo/hand-painted-watercolor-background-with-sky-clouds-shape_24972-1095.jpg?w=2000);
            background-size: cover;
            background-position: top center;
        }

        .home .image{
            flex:1 1 40rem;
        }

        .home .image img{
            width:100%;
        }

        .home .content{
            flex:1 1 40rem;
        }

        .home .content .hi{
            font-size: 2rem;
            color:var(--main-color);
        }

        .home .content h3{
            font-size: 4.5rem;
            color:rgb(3, 3, 3);    
        }

        .home .content h3 span{
            color:var(--main-color);   
        }

        .home .content .info{
            font-size: 2.5rem;
            color:rgb(53, 22, 226);
            padding:.5rem 0;
        }

        .home .content .text{
            font-size: 1.7rem;
            color:rgb(54, 18, 160);
            padding:.5rem 0;
        }

        .about .row-1{
            display: flex;
            flex-wrap: wrap;
            gap:1.5rem;
            padding-bottom: 2rem;
        }

        .about .row-1 .image{
            flex:1 1 25rem;
        }

        .about .row-1 .image img{
            height: 100%;
            width:100%;
            object-fit: cover;
            border:1rem solid #fff;
            border-radius: .5rem;
            box-shadow: 0 .5rem 1rem rgba(170, 42, 42, 0.1);
        }

        .about .row-1 .content{
            flex:1 1 50rem;
        }

        .about .row-1 .content h3{
            color:#333;
            font-size: 3.5rem;
        }

        .about .row-1 .content p{
            color:#666;
            font-size: 1.7rem;
            padding:.5rem 0;
        }

        .about .row-1 .content .box-container{
            display: flex;
            flex-wrap: wrap;
            gap:1.5rem;
            padding: 0.5rem 0;
        }

        .about .row-1 .content .box-container .box{
            flex:1 1 20rem;
        }

        .about .row-1 .content .box-container .box span{
            color:var(--main-color);
        }

        .about .row-2{
            display: flex;
            flex-wrap: wrap;
            gap:1.5rem;
            align-items: center;
        }

        .about .row-2 .skills{
            flex:1 1 40rem;
        }

        .about .row-2 .skills .progress{
            padding:1rem 0;
        }

        .about .row-2 .skills .progress h3{
            display: flex;
            justify-content: space-between;
            padding:.7rem 0;
            font-size: 1.7rem;
            color:#111;
            font-weight: 400;
        }

        .about .row-2 .skills .progress .bar{
            width:100%;
            background:#ccc;
            overflow:hidden;
            height:1rem;
            border-radius: 50rem;
        }

        .about .row-2 .skills .progress .bar span{
            display:block;
            height:100%;
            background:var(--main-color);
            border-radius: 50rem;
        }

        .about .row-2 .skills .progress:nth-child(1) .bar span{
            width:95%;
        }

        .about .row-2 .skills .progress:nth-child(2) .bar span{
            width:80%;
        }

        .about .row-2 .skills .progress:nth-child(3) .bar span{
            width:75%;
        }

        .about .row-2 .skills .progress:nth-child(4) .bar span{
            width:85%;
        }

        .about .row-2 .box-container{
            flex:1 1 40rem;
            display: flex;
            flex-wrap: wrap;
            gap:1.5rem;
        }

        .about .row-2 .box-container .box{
            flex:1 1 15rem;
            background:#fff;
            padding:2rem;
            border-radius: .5rem;
            box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
        }

        .about .row-2 .box-container .box h3{
            color:var(--main-color);
            font-size: 3rem;
        }

        .about .row-2 .box-container .box p{
            color:#666;
            font-size: 1.7rem;
            padding-top: .5rem;
        }

        .service .box-container{
            display: flex;
            flex-wrap: wrap;
            gap:1.5rem;
        }

        .service .box-container .box{
            flex:1 1 30rem;
            text-align: center;
            padding:2rem;
            background:#fff;
            border-radius: .5rem;
            box-shadow:0 .5rem 1rem rgba(0,0,0,.1);
        }

        .service .box-container .box i{
            height:6rem;
            width:6rem;
            line-height: 6rem;
            font-size: 2.5rem;
            color:#fff;
            background:var(--main-color);
            border-radius: 50%;
        }

        .service .box-container .box h3{
            color:#444;
            font-size: 2.2rem;
            padding-top: 1rem;
        }

        .service .box-container .box p{
            color:#666;
            font-size: 1.7rem;
            padding-top: .5rem;
        }

        .experience .box-container{
            display: flex;
            flex-wrap: wrap;
        }

        .experience .box-container .box{
            position: relative;
            flex:1 1 33rem;
            border-left: .2rem solid var(--main-color);
            padding-left: 2rem;
            padding-right: 2rem;
            padding-bottom: 2rem;    
        }

        .experience .box-container .box::before{
            content: '';
            position: absolute;
            top:0; left:-1rem;
            height:2rem;
            width:2rem;
            border-radius: 50%;
            background:var(--main-color);
        }

        .experience .box-container .box .content{
            background:#fff;
            padding:1.5rem;
            box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
            border-radius: .5rem;
        }

        .experience .box-container .box .content span{
            color:#fff;
            font-size: 1.7rem;
            background:var(--main-color);
            border-radius: 50rem;
            padding:.4rem 1rem;
        }

        .experience .box-container .box .content h3{
            font-size: 2.5rem;
            padding:.5rem 0;
            color:#111;
        }

        .experience .box-container .box .content p{
            font-size: 1.5rem;
            color:#666;
        }

        .portfolio .box-container{
            display: flex;
            flex-wrap: wrap;
            gap:1.5rem;
        }

        .portfolio .box-container .box{
            flex:1 1 30rem;
            height:25rem;
            position: relative;
            overflow:hidden;
            border:1rem solid #fff;
            box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
            background:#fff;
            border-radius: .5rem;
        }

        .portfolio .box-container .box img{
            height:100%;
            width:100%;
            object-fit: cover;
            border-radius: .5rem;
            position: relative;
            z-index: 1;
        }

        .portfolio .box-container .box:hover img{
            height:75%;
            width:75%;
        }

        .portfolio .box-container .box h3{
            position: absolute;
            bottom:.5rem; left:1rem;
            font-size: 2.5rem;
            color:#333;
            text-transform: uppercase;
        }

        .portfolio .box-container .box .icons{
            position: absolute;
            top:1rem; right:1rem;
        }

        .portfolio .box-container .box .icons a{
            display: block;
            height:4rem;
            width:4rem;
            border-radius: .5rem;
            background: #eee;
            color:#333;
            font-size: 1.7rem;
            line-height: 4rem;
            text-align: center;
            margin-bottom: 1rem;
        }

        .portfolio .box-container .box .icons a:hover{
            background:var(--main-color);
            color:#fff;
        }

        .contact .icons-container{
            display: flex;
            gap:1.5rem;
            flex-wrap: wrap;
            padding-bottom: 2rem;
        }

        .contact .icons-container .icons{
            flex:1 1 25rem;
            text-align: center;
            padding:2rem;
            background:#fff;
            box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
            border-radius: .5rem;
        }

        .contact .icons-container .icons i{
            height:5rem;
            width:5rem;
            line-height: 5rem;
            font-size: 2rem;
            background: var(--main-color);
            color:#fff;
            border-radius: 50%;
        }

        .contact .icons-container .icons h3{
            color:#111;
            font-size: 2rem;
            padding:.5rem 0;
            padding-top: 1rem;
        }

        .contact .icons-container .icons p{
            color:#666;
            font-size: 1.7rem;
        }

        .contact .row{
            display: flex;
            flex-wrap: wrap;
            gap:1.5rem;
        }

        .contact .row form{
            flex:1 1 55rem;
            background:#fff;
            padding:0 2rem;
            box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
            border-radius: .5rem;
        }

        .contact .row .map{
            flex:1 1 25rem;
            border:1rem solid #fff;
            box-shadow: 0 .5rem 1rem rgba(0,0,0,.1);
            border-radius: .5rem;
            width: 100%;
        }

        .contact .row form .box,
        .contact .row form textarea{
            width: 100%;
            border-bottom: .1rem solid #333;
            color:#333;
            text-transform: none;
            font-size: 1.7rem;
            padding:1rem 0;
            margin:1rem 0;
        }

        .contact .row form .box:focus,
        .contact .row form textarea:focus{
            border-color: var(--main-color);
        }

        .contact .row form .box::placeholder,
        .contact .row form textarea::placeholder{
            text-transform: capitalize;
        }

        .contact .row form textarea{
            height: 20rem;
            resize: none;
        }

        .contact .row form .btn{
            margin-top: 0;
            margin-bottom: 1.5rem;
        }

        .footer{
            margin-top: 2rem;
            font-size: 2rem;
            padding:2.5rem;
            text-align: center;
            color:#666;
            background: #fff;
        }

        .footer span{
            color:var(--main-color);
        }


        /* media queries  */
        @media (max-width:991px){

            html{
                font-size: 55%;
            }
            
            body{
                padding: 0;
            }

            #menu-bars{
                display: initial;
            }

            header{
                left:-120%;
            }

            header.active{
                left:0%;
            }

            .cursor-1,
            .cursor-2{
                display: none;
            }

        }

        @media (max-width:450px){

            html{
                font-size: 50%;
            }

            header{
                width:100%;
            }

            .experience .box-container .box{
                padding-right: 0;
            }

        }
    </style>

</head>
<body>

<!-- custom cursors  -->
<div class="cursor-1"></div>
<div class="cursor-2"></div>


<div id="menu-bars" class="fas fa-bars"></div>
    
<!-- header section starts  -->

<header>

    <a href="https://tse2.mm.bing.net/th?id=OIP.JDSoQIUEHEYgf7IGjGS5DQHaEK&pid=Api&P=0" class="logo"> <span>VISHNU</span> VEERAPU </a>

    <nav class="navbar">
        <a href="#home">home</a>
        <a href="#about">about</a>
        <a href="#service">Skills</a>
        <a href="#experience">experience</a>
        <a href="#contact">contact</a>
    </nav>

    <div class="follow">  
        <a href="https://instagram.com/vishnu_veerapu?igshid=YmMyMTA2M2Y=" target="_blank" class="fab fa-instagram"></a>
    </div>

</header>

<!-- header section ends -->

<!-- home section starts  -->

<section class="home" id="home">

    <div class="content">
        <span class="hi"> hi there... </span>
        <h3> i am <span> VISHNU</span> </h3>
        <p class="info"> Fighter </p>
        <p class="text"> I am from Pulivendula,ANDHRA PRADESH.
            I'm Fresher in VIT-AP university.I  have taken  Computer Science  Engineering
            in Btech.I'm dedicated,hardworking student.I'm good at organizing things.My hobbies 
            are  reading books,listening music etc.I am interseted in learning new things.I always                   
            beleive in myself.Recently I have joined in Csi club.I'm happy to to be apart of this club. </p>
        <a href="#about" class="btn">about me</a>
        
    </div>
    <div class="image">
        <img src="images/home-img.png" alt="">
    </div>

</section>

<!-- home section ends -->

<!-- about section starts  -->

<section class="about" id="about">

<h1 class="heading"> about <span> me </span> </h1>

<div class="row-1">

    <div class="image">
        <img src="C:\Users\vishn\Desktop\WhatsApp Image 2022-08-16 at 7.39.18 PM.jpeg" alt="">
    </div>

    <div class="content">
        <h3>My name is Vishnu</h3>
        <p>My hobbies are Scrolling Insta ,listening music, Reading etc.I am interseted in learning new things.</p>
        <div class="box-container">
            <div class="box">
                <p> <span> language : </span> Telugu, Hindi, English,French </p>
                <p> <span> work : </span> Student </p>
            </div>
            <div class="box">
                <p> <span> phone : </span> 7780648597 </p>
                <p> <span> email : </span> vishnuveerapu@gmail.com </p>  
            </div>
        </div>
        <a href="#" class="btn">download CV</a>
    </div>

</div>

<h1 class="heading"> <span> i'am </span> Good at </h1>

<div class="row-2">

    <div class="skills">
        <div class="progress">
            <h3> web design <span> 7% </span> </h3>
            <div class="bar"> <span></span> </div>
        </div>
        <div class="progress">
            <h3> web development <span> 10% </span> </h3>
            <div class="bar"> <span></span> </div>
        </div>
        <div class="progress">
            <h3> UI design <span> 40% </span> </h3>
            <div class="bar"> <span></span> </div>
        </div>
        <div class="progress">
            <h3> stock marketing <span> 70% </span> </h3>
            <div class="bar"> <span></span> </div>
        </div>
    </div>

    <div class="box-container">

        <div class="box">
            <h3>Begginner  </h3>
            <p>in learning</p>
        </div>
        <div class="box">
            <h3> >> 1+ </h3>
            <p>projects completed</p>
        </div>

    </div>

</div>

</section>

<!-- about section ends -->

<!-- service section starts  -->

<section class="service" id="service">

<h1 class="heading"> <span> my </span> Skills </h1>

    <div class="box-container">

        <div class="box">
            <i class="fas fa-code"></i>
            <h3>communication</h3>
            <p>good at communication </p>
        </div>

        <div class="box">
            <i class="fas fa-paint-brush"></i>
            <h3>Editing</h3>
            <p>good in editing images</p>
        </div>

        <div class="box">
            <i class="fas fa-mobile"></i>
            <h3>technical knowledge</h3>
            <p>good in technical skillls</p>
        </div>

        <div class="box">
            <i class="fas fa-bullhorn"></i>
            <h3>stock marketing</h3>
            <p>leadership skills</p>
        </div>

        <div class="box">
            <i class="fas fa-chart-line"></i>
            <h3>time management</h3>
            <p>good in managing time wisely</p>
        </div>

        <div class="box">
            <i class="fas fa-envelope"></i>
            <h3>creativity</h3>
            <p>good in creative skills</p>
        </div>

    </div>

</section>

<!-- service section ends -->

<!-- experience section starts  -->

<section class="experience" id="experience">

    <h1 class="heading"> <span> my </span> experience </h1>

    <div class="box-container">

        <div class="box">
            <div class="content">
                <span> 2021 - 2022 </span>
                <h3>python</h3>
                <p>beginner</p>
            </div>
        </div>

        <div class="box">
            <div class="content">
                <span> 2021 - 2022 </span>
                <h3>java</h3>
                <p>beginner</p>
            </div>
        </div>

        <div class="box">
            <div class="content">
                <span> 2021 - 2022 </span>
                <h3>html and css</h3>
                <p>beginner</p>
            </div>
        </div>

        <div class="box">
            <div class="content">
                <span> 2021 - 2022 </span>
                <h3>c</h3>
                <p>beginner</p>
            </div>
        </div>

        

    </div>

</section>

<!-- experience section ends -->

<!-- contact section starts  -->

<section class="contact" id="contact">

    <h1 class="heading"> contact <span> me </span> </h1>

    <div class="icons-container">

        <div class="icons">
            <i class="fas fa-envelope"></i>
            <h3>my email</h3>
            <p>vishnuveerapu@gmail.com</p>
        </div>

        <div class="icons">
            <i class="fas fa-phone"></i>
            <h3>my number</h3>
            <p>7780648597</p>
        </div>

        <div class="icons">
            <i class="fas fa-map-marker-alt"></i>
            <h3>my address</h3>
            <p>andhra pradesh</p>
        </div>

    </div>

    <div class="row">

        <form action="">

            <input type="text" placeholder="name" class="box">
            <input type="email" placeholder="email" class="box">
            <input type="number" placeholder="number" class="box">

            <textarea name="" placeholder="message" id="" cols="30" rows="10"></textarea>

            <input type="submit" class="btn" value="send message">

        </form>

    </div>


</section>

<!-- contact section ends -->

<!-- footer section  -->
<footer class="footer"> created by <span>vishnu</span> | all rights reserved! </footer>

</body>
</html>
