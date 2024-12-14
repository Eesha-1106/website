# Ex.07 Restaurant Website
# Date:8-11-2024
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
```
website.html:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurant Website</title>
    <link rel="stylesheet" href="C:\Users\admin\Documents\html\style.css">
</head>
<body>
    <section id="Home">
        <nav>
            <div class="logo">
                <img class="image" src="Flavors of india.jpeg" width="10%"style="display:block;margin-left: auto;margin-right: auto;background-blend-mode: lighten;background-color: inherit;"/>
            </div>
            <ul>
                <li><button class="btn" type="button" onclick="location.href='website.html'">Home</a></li>
                <li><button class="btn" type="button" onclick="location.href='About.html'">About</a></li>
                <li><button class="btn" type="button" onclick="location.href='menu.html'">Menu</a></li>
                <li><button class="btn" type="button" onclick="location.href='contact us.html'">Contact us</a></li>
            </ul>
        </nav>
        <div class="main" id="Home" >
            <div class="main_text">
                <h1 style="font-family:'Times New Roman', Times, serif">  Flavors Of India</h1>
                <h1 style="color:burlywood;left:300px;text-align: center;">.</h1>
                <h2>   Savour The Flavor...</h2>
                <h2>   ...Love The Experience</h2>
                <h1 style="color:burlywood;left:300px;text-align: center;">.</h1>
                <h3  style="font-family:cursive;font-style:italic">   North Indian, South Indian, Oriental, continental,Mexican,Italian,Chinese,Desserts,Beverages</h3>
            </div>
            <div class="main_image">
                <img src="C:\Users\admin\Documents\html\restaurant img.avif">
            </div>
        </div>     
    </section>
</body>
</html>

style.css:
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}
html{
    scroll-behavior: smooth;
}
section{
    width: 100%;
    height:100vh;
}
section nav{
    display:flex;
    justify-content:space-around;
    align-items:center;
    position:fixed;
    right:0;
    left:0;
    background:url('WhatsApp Image 2024-10-20 at 2.44.26 PM.jpeg');
    box-shadow: 0 0 10px rgba(0,0,0,0.5);
    z-index:1000;
}
section nav .logo img{
    width:100px;
    cursor:pointer;
    margin:7px 0;
}
section nav ul{
    list-style:none;
}
section nav ul li{
    display:inline-block;
    margin:0 15px;

}
.btn{
    padding:15px 30px;
    border:none;
    outline:none;
    color:rgb(235, 177, 101);
    cursor:pointer;
    position:relative;
    z-index:0;
    border-radius:12px;
    font-family:Arial, Helvetica, sans-serif
    transition:0.1s;
}
.btn::after{
    content:"";
    z-index:-1;
    position:absolute;
    width:100%;
    height:100%;
    background-color:rgb(29, 0, 0);
    left:0;
    top:0;
    border-radius: 10px;
    display: block;
    transition: 0.2 linear;
}
.btn:hover::after{
    width:100%;
}
.btn:hover{
    color:rgb(214, 142, 54);
}
section .main{
    display: flex;
    align-items: center;
    justify-content: space-around;
    position: relative;
    top:115px;
}
section .main .main_text h1{
    font-size: 70px;
    position: relative;
    color:rgb(39, 2, 2);
    left:40px;
}
section .main .main_text h2{
    font-size:50px;
    position: relative;
    color:rgb(170, 115, 13);
    left:70px;   
}
section .main .main_text h3{
    font-size:20px;
    position: relative;
    color:rgb(170, 115, 13);
    left:70px
}
section .main .main_image{
    max-width: 50%;   
}
section .main .main_image img{
    width: 100%;
    height:auto;
}
section .about{
    display: flex;
    flex-wrap: wrap;
    align-items:center;
    justify-content: center;
    position: relative;
    top:115px;
    padding: 20px;
    overflow:hidden;
}
section .about .about_image{
    max-width:100%;
    text-align: start;

}
section .about .about_image img{
    width:100%;
    height:auto;
   
}
section .about .about_text{
    flex:1;
    max-width:100%;
    padding:65px;
    text-align:center;
    overflow: hidden;

}
section .about .about_text h1{
    font-size: 70px;
    flex:1;
    position:relative;
    color:rgb(170, 115, 13);
    min-width: 300px;
    padding:20px;
    text-align: center;
    
}
section .about .about_text h3,p{
    font-size:30px;
    position: relative;
    color:rgb(104, 44, 16);
    font-family:'Courier New', Courier, monospace;
    margin-bottom:20px;
}

about.html:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurant Website</title>
    <link rel="stylesheet" href="C:\Users\admin\Documents\html\style1.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css" integrity="sha512-Kc323vGBEqzTmouAECnVceyQqyqdsSiqLQISBL29aUW4U/M7pSPA/gEUZQqv1cwx4OnYxTxve5UMg5GT6L4JJg==" crossorigin="anonymous" referrerpolicy="no-referrer" />
</head>
<body >
    <section >
        <nav>
            <div class="logo">
                <img class="image" src="Flavors of india.jpeg" width="10%"style="display:block;margin-left: auto;margin-right: auto;background-blend-mode: lighten;background-color: inherit;"/>
            </div>

            <ul>
                <li><button class="btn" type="button" onclick="location.href='website.html'">Home</a></li>
                <li><button class="btn" type="button" onclick="location.href='About.html'">About</a></li>
                <li><button class="btn" type="button" onclick="location.href='menu.html'">Menu</a></li>
                <li><button class="btn" type="button" onclick="location.href='contact us.html'">Contact us</a></li>
            </ul>
        </nav>
        <div class="main" >
            <div class="main_image">
                <img src="C:\Users\admin\Documents\html\WhatsApp Image 2024-10-21 at 8.34.53 AM.jpeg" >
            </div>
            <div class="main_text">
                <h1 style="font-family:'Courier New', Courier, monospace;font-style:italic;color:  rgb(39, 2, 2)">About Us...</h1>
                <h3>Service options: Has all you can eat · Serves vegan dishes · Good for kids birthday</h3>
                <h3>Address:1st Floor Above Dominoe's E Block CitY center Bengaluru-560103</h3>
                <h3>Phone: 098436 32323</h3>
                <h3>From Flavors Of India
                    " a pure veg multicuisine restaurant situated in kilpauk area of Chennai City, Tamil Nadu."</h3>
            </div>
        </div>
        </div>
        </section>
 style1.css:
section .main{
    display: flex;
    gap:30px;
    padding:20px;
    flex-wrap:wrap;
    align-items:center;
    justify-content: center;
    position: relative;
    top:115px;
    background-repeat: no-repeat;
    background-size:cover;
}
section .main .main_image{
    max-width:100%;
    flex-shrink: 0;
}
section .main .main_image img{
    width:100%;
    height:auto;
    display:block;
}
section .main .main_text{
    flex:1;
    max-width:100%;
    padding:65px;
    text-align:center;
    overflow:hidden;
}
section .main .main_text h1{
    font-size: 70px;
    flex:1;
    position: relative;
    color:rgb(170, 115, 13);
    min-width:300px;
    padding:20px;
    text-align:center;
}
section .main .main_text h3,p{
    font-size:30px;
    position: relative;
    color:rgb(104, 44, 16);
    font-family:'Courier New', Courier, monospace;
    margin-bottom: 20px;
}
menu.html:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurant Website</title>
    <link rel="stylesheet" href="C:\Users\admin\Documents\html\style2.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css" integrity="sha512-Kc323vGBEqzTmouAECnVceyQqyqdsSiqLQISBL29aUW4U/M7pSPA/gEUZQqv1cwx4OnYxTxve5UMg5GT6L4JJg==" crossorigin="anonymous" referrerpolicy="no-referrer" />
</head>
<body >
    <section id="Home">
        <nav>
            <div class="logo">
                <img class="image" src="Flavors of india.jpeg" width="10%"style="display:block;margin-left: auto;margin-right: auto;background-blend-mode: lighten;background-color: inherit;"/>
            </div>

            <ul>
                <li><button class="btn" type="button" onclick="location.href='website.html'">Home</a></li>
                <li><button class="btn" type="button" onclick="location.href='About.html'">About</a></li>
                <li><button class="btn" type="button" onclick="location.href='menu.html'">Menu</a></li>
                <li><button class="btn" type="button" onclick="location.href='contact us.html'">Contact us</a></li>
            </ul>
        </nav>
        <div class="menu">
            <div class="heading">
                <h1>RESTAURANT FOOD</h1> 
                <h3>&mdash;MENU&mdash;</h3>
            </div>
            <div class="food-items">
                <img src="C:\Users\admin\Documents\html\Paneer-Tikka-Featured.jpg"/>
                <div class="detals">
                    <div class="detailed-sub">
                        <h5>Paneer Tikka</h5>
                    </div>
                    <p>cubes of paneer & veggies marinated with yogurt and spices. Traditionally it's grilled in a tandoor </p>
                    
                </div>
            </div>
            <div class="food-items">
                <img src="C:\Users\admin\Documents\html\veg-manchurian.jpg"/>
                <div class="detals">
                    <div class="detailed-sub">
                        <h5>Veg Manchurian</h5>
                    </div>
                    <p>a vegetarian Indo-Chinese dish in which shredded vegetables are formed to balls and fried until crisp. </p>
                    
                </div>
            </div>
            <div class="food-items">
                <img src="C:\Users\admin\Documents\html\veg-fried-rice-recipe.jpg"/>
                <div class="detals">
                    <div class="detailed-sub">
                        <h5>Veg Fried Rice</h5>
                    </div>
                    <p>classic Veg Fried Rice recipe is made with a hearty mix of fresh vegetables, green onions, seasonings and spices for an incredibly flavorful fried rice dish.</p>
                </div>
            </div>
        
            <div class="food-items">
                <img src="C:\Users\admin\Documents\html\noodles_food_1.jpg"/>
                <div class="detals">
                    <div class="detailed-sub">
                        <h5>Veg Noodles</h5>
                    </div>
                    <p>a healthy Chinese inspired dish where cooked noodles are stir fried with lots of vegetables.</p>
                    
                </div>
            </div>
            <div class="food-items">
                <img src="C:\Users\admin\Documents\html\FB-Thumnails-website-old-66.jpg"/>
                <div class="detals">
                    <div class="detailed-sub">
                        <h5>Naan</h5>
                    </div>
                    <p>a leavened, oven-baked flatbread that is a staple of South and Central Asian cuisine </p>
                    
                </div>
            </div>
            <div class="food-items">
                <img src="C:\Users\admin\Documents\html\AR-24878-bbq-chicken-pizza-beauty-2x1-bdc59852305a41cf8f98c6c15e8b540c.jpg"/>
                <div class="detals">
                    <div class="detailed-sub">
                        <h5>Pizza</h5>
                    </div>
                    <p>cubes of paneer & veggies marinated with yogurt and spices. Traditionally it's grilled in a tandoor </p>
                   
                </div>
            </div>
            <div class="food-items">
                <img src="C:\Users\admin\Documents\html\paneer-butter-masala-recipe-2.jpg"/>
                <div class="detals">
                    <div class="detailed-sub">
                        <h5>Paneer Butter Masala</h5>
                    </div>
                    <p>a rich and creamy dish of paneer (Indian cottage cheese) in a tomato, butter and cashew sauce that is known here as “makhani gravy.</p>
                    
                </div>
            </div>
            <div class="food-items">
                <img src="C:\Users\admin\Documents\html\falooda-featured.jpg"/>
                <div class="detals">
                    <div class="detailed-sub">
                        <h5>Falooda</h5>
                    </div>
                    <p>a cold, layered dessert or snack that originated in Persia and is popular in India, Pakistan, and the Middle East </p>
                    
                </div>
            </div>
            <div class="food-items">
                <img src="C:\Users\admin\Documents\html\images (1).jfif"/>
                <div class="detals">
                    <div class="detailed-sub">
                        <h5>Coconut Payasam</h5>
                    </div>
                    <p>silky smooth dessert made by simmering milk with tender coconut water, tender coconut pulp, sugar, condensed milk and flavored with cardamom powder</p>
                    
                </div>
            </div>
        </div>
    </section>
    </body>
</html>

style2.css:

section .menu{
    display: flex;
    align-items: center;
    justify-content: space-around;
    position: relative;
    top:115px;
    padding:0 10px 30px 10px;
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(350px,1fr));
    grid-gap:20px 40px;
}
section .menu .heading{
    color:brown;
    margin: bottom 30px;
    padding:30px 0;
    grid-column:1/-1;
    text-align:center;
}
section .menu .food-items{
    display:grid;
    position:relative;
    grid-template-rows:auto 1fr;
    border-radius:15px;
    box-shadow:0 0 15px rgba(0,0,0,0.5);
    transition:.2s ease-in-out;
}
section .menu .food-items img{
    position:relative;
    width:100%;
    height:280px;
    border-radius:15px 15px 0 0;
    cursor:pointer;
}
section .menu .heading h1{
    grid-column:1/-1;
    text-align:center
}
section .menu .food-items .details{
    padding:20px 10px;
    display:grid;
    grid-template-rows:auto 1fr 50px;
    grid-row-gap:15px;
}

contact us.html:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurant Website</title>
    <link rel="stylesheet" href="C:\Users\admin\Documents\html\style3.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css" integrity="sha512-Kc323vGBEqzTmouAECnVceyQqyqdsSiqLQISBL29aUW4U/M7pSPA/gEUZQqv1cwx4OnYxTxve5UMg5GT6L4JJg==" crossorigin="anonymous" referrerpolicy="no-referrer" />
</head>
<body >
    <section >
        <nav>
            <div class="logo">
                <img class="image" src="Flavors of india.jpeg" width="10%"style="display:block;margin-left: auto;margin-right: auto;background-blend-mode: lighten;background-color: inherit;"/>
            </div>
            <ul>
                <li><button class="btn" type="button" onclick="location.href='website.html'">Home</a></li>
                <li><button class="btn" type="button" onclick="location.href='About.html'">About</a></li>
                <li><button class="btn" type="button" onclick="location.href='menu.html'">Menu</a></li>
                <li><button class="btn" type="button" onclick="location.href='contact us.html'">Contact us</a></li>
            </ul>
        </nav>
        <div class="main" >
            <div class="main_image">
                <img src="C:\Users\admin\Documents\html\falvors map.PNG" >
            </div>
            <div class="main_text">
                <h1 style="font-family:'Courier New', Courier, monospace;font-style:italic;color:  rgb(39, 2, 2)">Contact us</h1>
                <h3>Address:1st Floor Above Dominoe's E Block CitY center Bengaluru-560103</h3>
                <h3>Phone: 098436 32323</h3>
                <h3>Hours:11.AM-11.30PM</h3>
                <h3>Reservations: zomato.com</h3>
            </div>
        </div>
        </div>
        </section>

style3.css:

section .main{
    display: flex;
    gap:30px;
    padding:20px;
    flex-wrap:wrap;
    align-items:center;
    justify-content: center;
    position: relative;
    top:115px;
    background-repeat: no-repeat;
    background-size:cover;
}
section .main .main_image{
    max-width:100%;
    flex-shrink: 0;
}
section .main .main_image img{
    width:100%;
    height:auto;
    display:block;
}
section .main .main_text{
    flex:1;
    max-width:100%;
    padding:65px;
    text-align:center;
    overflow:hidden;
}
section .main .main_text h1{
    font-size: 70px;
    flex:1;
    position: relative;
    color:rgb(170, 115, 13);
    min-width:300px;
    padding:20px;
    text-align:center;   
}
section .main .main_text h3,p{
    font-size:30px;
    position: relative;
    color:rgb(104, 44, 16);
    font-family:'Courier New', Courier, monospace;
    margin-bottom: 20px;
}

```
# OUTPUT:
![Capture web](https://github.com/user-attachments/assets/a37bb5d9-268c-490c-a347-43ab77288053)
![Capture web1](https://github.com/user-attachments/assets/2d171486-84e1-43bc-8835-8d8530f6fbfc)
![Capture web2](https://github.com/user-attachments/assets/076b0d85-4fbc-4e4d-95e4-d970936b9e23)
![Capture web3](https://github.com/user-attachments/assets/f2c4fe28-1478-4da0-8c41-789f88bcd7f7)
![Capture web4](https://github.com/user-attachments/assets/20feafa1-ccc7-4a98-a938-0d2ffe088eb7)

# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
