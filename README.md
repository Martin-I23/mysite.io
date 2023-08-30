<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hanoi - Exploring The City</title>
    <link rel="stylesheet" href="hanoi.css">
    <link rel="stylesheet" href="hanoi.js">
    <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
<link href="https://cdn.jsdelivr.net/npm/remixicon@2.2.0/fonts/remixicon.css" rel="stylesheet">
<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/all.min.css" rel="stylesheet">
</head>

<style>

  *{
    box-sizing: border-box;
    padding: 0;
    margin: 0;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.navbar{
    background-color: black;
    overflow: hidden;
}

.navbar a{
    color: yellow;
    font-size: 21px;
    padding: 19px 21px;
    display: inline-block;
    text-decoration: none;
    padding-left: 2%;
    padding-right: 2%;
}

.navbar a:hover{
    color: red;
}

.navbar h2.logo{
    font-size: 30px;
    color: white;
    float: right;
    cursor: pointer;
    margin-right: 30px;
    transform: translateY(10px);
}

.sidebar{
    overflow-x: hidden;
    background-color: black;
    color: rgb(246, 250, 5);
    width:0;
    height: 100%;
    top:0;
    box-shadow: 2px 2px 2px 2px rgb(39, 39, 39);
    position: fixed;
    left:0;
    z-index: 2;
    }
    
    .sidebar a{
    padding: 20px;
    font-size: 21px;
    color: white;
    text-shadow: 1px 2px 1px 1px rgb(243, 242, 243);
    display: block;
    text-decoration: none;
    }
    
    .sidebar a:hover{
    color: rgb(167, 4, 4);
    }
    
    .sidebar .closebtn{
    right: 60px;
    margin-left: 160px;
    font-size: 21px;
    }
    
    

.header{
    background-attachment: fixed;
    background-repeat: no-repeat;
    background-size: cover;
    padding: 20px;
    height: 500px;
    width: 100%;
    background-position: center;
    background-image: linear-gradient(rgba(221, 9, 9, 0), rgba(,0,0,0,0.9)), url(hanoi.jpg);
}

h1.title{
    margin-left: 50px;
    color: white;
    font-size: 50px;
    padding: 30px;
}

h3.explain{
    color: aliceblue;
    margin-left: 60px;
    padding: 30px;
    font-size: 36px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-style: oblique;
    font-weight: 500;
}

button{
    color: yellow;
    width: 190px;
    outline: none;
    padding: 12px 0px;
    border-radius: 30px;
    background-color: red;
    border: 0; 
    margin-left: 80px;
    text-align: center;
    font-size: 19px;
    cursor: pointer;
    margin-top: 50px;
    font-weight: 700;
    transition: 0.5s;
}

button:hover{
    background-color: yellow;
    color: red;
}

marquee{
    background: black;
    color: yellow;
    padding: 23px 25px;
}

.row{
    display: flex;
    flex-wrap: flex;
}

.sideleft{
    flex: 25%;
    padding: 20px;
    background-color: black;
    color: aliceblue;
}

.container{
    width: 100%;
    height: 400px;
    border: 0;
    align-items: center;
    font-size: 25px;
    padding: 30px;
    cursor: pointer;
    background-color: red;
}

.container-second{
    border: 2px solid yellow;
    margin-top: 50px;
   height: 300px;
   padding: 20px;
   color: yellow;   
}

.container a{
    text-align: center;
    text-decoration: none;
    display: block;
    color: white;
}

.container a:hover{
    color: yellow;
}

.main{
    color: aliceblue;
    flex: 50%;
    background-color: black;
    padding: 20px;
}

h4.m-title{
    font-size: 36px;
  }

  .fs{
    flex-basis: 50%;
    display: flex;
    margin-top: 40px;
  }

  .texting p{
    font-size: 16px;
    line-height: 20px;
    letter-spacing: 0.7px;
    margin-top: 50px;
   font-family: sans-serif; 
   font-weight: 600;
}

hr{
    width: 50%;
    border: 2px solid yellow;
}

.social-media{
    margin-top: 50px;
}

.social-media a{
    color: white;
    text-decoration: none;
    font-size: 30px;
    display: inline-block;
    padding: 13px 15px;
}

.social-media a:hover{
    color: yellow;
}

.sideright{
    color: aliceblue;
    padding: 20px;
    background-color: black;
    flex: 25%;
}

h3.r-title{
    font-size: 36px;
  }

  .container-thirth{
    width: 100%;
    padding: 20px;
    flex: 1;
    height: auto;
    border: 2px solid red;
    margin-top: 600px;
  }

  .container-thirth .linking a{
    color: red;
    font-size: 21px;
    text-decoration: none;
    padding: 12px 15px;
    display: block;
    transition: 0.5s;
  }

  .container-thirth .linking a:hover{
    color: yellow;
    text-decoration: underline;
  }

  .footer{
    border-top: 2px solid white;
    text-align: center;
    text-align: center;
    color: rgb(255, 255, 255);
    clear: both;
    background-color: black;
    width: 100%;
    padding: 20px;
    height: 30%;
    font-size: 14px;
  }

  
::-webkit-scrollbar{
    width: 10px;
   }
   
   ::-webkit-scrollbar-track{
   background-color: black;
   }
   
   ::-webkit-scrollbar-thumb{
    background-image: linear-gradient(rgb(255, 196, 0), rgb(255, 2, 2));
   border-radius: 10px;
   box-shadow: 2px 2px 2px 2px rgb(187, 27, 27);
   }

</style>
  
<body>
    <div class="navbar">
        <div class="sidebar" id="myside">
            <a href="javascript:void(0)" onclick="closeNav()" class="closebtn">&times;</a>
            <h2 style="color:white; padding: 20px; text-shadow: 1px 2px 1px 1px rgb(230, 255, 4);">See our recommendations:</h2>
            <br>
            <hr style="border: 1px solid rgb(251, 255, 3);">
            <a href="#">Facts</a>
            <a href="#">Interesting Places</a>
            <a href="#">Pagoda</a>
            <a href="#">Nightlife</a>
            <a href="#">Exploring</a>
            <a href="#">Other Cities</a>
            <br>
            <hr style="border: 1px solid rgb(248, 244, 4);">
            <p style="color:white; padding: 20px; padding: 20px; font-size: 13px; text-shadow: 1px 2px 1px 1px purple;">City Music is a corporative site where you can see a lot of different music styles for listening. Dont't hesitate and start enjoying time with your favourite mix.</p>
            <br>
            <p style="font-size: 11px; color: white; text-align: center; padding: 20px;">Copyright 2023<sup><i class="ri-copyright-line"></i></sup> City Music</p>
            </div>
            <span style="font-size: 30px; color: white; margin: 5px; padding: 20px; cursor:pointer; margin-left: 10px;" onclick="openNav()"><i class="ri-menu-2-line"></i></span>

        <a href="file:///C:/Users/Ico/OneDrive/Escritorio/carpetas/Greece/elinika.html">Greece</a>
        <a href="file:///C:/Users/Ico/OneDrive/Escritorio/carpetas/India/india.html">India</a>
        <a href="file:///C:/Users/Ico/OneDrive/Escritorio/carpetas/website/website.html">Philipines</a>
        <a href="">More</a>
        <h2 class="logo">XiNang</h2>
    </div>
    <div class="header">
        <h1 class="title">Explore the beautiful amount of pagoda!</h1>
        <h3 class="explain">You want to learn more about pagoda style!<br>Just click the button below.</h3>
        <button type="button">Explore Pagoda</button>
    </div>
    <div class="moving-line">
        <marquee position="scroll">Welcome
             to Hanoi City. Explore the beautiful temples, parks, lakes, the city center and the unmissing pagoda as well! If you have some question don't hesitate to ask us. We'll be sure to help you! Go below and take a look to one of the best cities in the entire Asia. You won't be disappointed!</marquee>
    </div>
    <div class="row">
        <div class="sideleft">
            <div class="container">
                <a>Hanoi In English</a>
                <br><br>
                <a>Hanoi In Vietnamese</a>
                <br><br>
                <a>Hanoi In Chinese</a>
                <br><br>
                <a href="#">Hanoi In Portuguese</a>
            </div>
            <br><br>
            <div class="container">
                <a>Hanoi In Bulgarian</a>
                <br><br>
                <a>Hanoi In Hindi</a>
                <br><br>
                <a>Hanoi In Korean</a>
                <br><br>
                <a href="#">Hanoi In Japanese</a>
            </div>
            <br><br>
            <div class="container">
                <a>Hanoi In German</a>
                <br><br>
                <a>Hanoi In Spanish</a>
                <br><br>
                <a>Hanoi In Italian</a>
                <br><br>
                <a href="#">Hanoi In French</a>
            </div>
            <div class="container-second">
                <h2>Interesting Fact</h2>
                <br>
                <p style="font-weight: 600;">One of the most famous and beloved street food delicacies in Hanoi is "Pho," a traditional Vietnamese noodle soup. Pho is typically made with a rich and aromatic broth, rice noodles, and either beef or chicken, garnished with fresh herbs, lime, chili, and bean sprouts. </p>
                <div class="container-thirth">
                <h1>Look our recommended websites below:</h1><br><br>
                <div class="linking">
                    <a href="https://historicalvision9.wordpress.com/">historicalvision9</a>
                    <a href="file:///C:/Users/Ico/OneDrive/Escritorio/WorldSports/signin.html">WorldSports</a>
                    <a href="file:///C:/Users/Ico/OneDrive/Escritorio/City%20Music/citylogin.html">CityMusic</a>
                   </div>
                </div>
            </div>
        </div>
        <div class="main">
            <h4 class="m-title">Hanoi City - The Vietnamese Cpital</h4>
            <img class="fs" src="first.jpg" width="100%" height="400px">

            <div class="texting">
                <p>Hanoi is the capital city of Vietnam and one of the country's most vibrant and historically significant cities. Here are some key details about Hanoi:</p><br><br><br>
                <h2 style="color: white; font-size: 36px;">1. Location</h2><br><hr><br>
                
                <img src="city.jpg" width="100%" height="400px">
                <p>Hanoi is located in the northern part of Vietnam, along the banks of the Red River. It is situated about 1,760 km (1,092 miles) north of Ho Chi Minh City (formerly Saigon), the country's largest city.</p><br><br><br>
                <h2 style="color: white; font-size: 36px;">2. History and Culture</h2><br><hr>
                 <p>Hanoi has a rich history that dates back over a thousand years. It was originally founded as Thang Long in 1010 during the Ly dynasty and served as the capital of Vietnam for various periods under different dynasties. In 1831, the city was renamed Hanoi, which means "inside the river," to reflect its location between the Red River and To Lich River.

                    <br><br>The city's culture is deeply influenced by a blend of Chinese, French, and Southeast Asian traditions.<br><br> This cultural diversity is evident in its architecture, cuisine, and festivals. Hanoi's Old Quarter is particularly famous for its narrow streets, colonial-era buildings, and bustling markets.</p> <br><br><br>
                    <h2 style="color: white; font-size: 36px;">3. Attractions</h2><br><hr><br>
                    <img src="attractions.jpg" width="100%" height="400px">

                    <p>Hanoi boasts numerous historical and cultural landmarks. Some of the most notable ones include the Ho Chi Minh Mausoleum, Hoan Kiem Lake (Lake of the Restored Sword), the Temple of Literature, One Pillar Pagoda, and the Hanoi Opera House.<br><br> The city's museums, like the Vietnam Museum of Ethnology and the Vietnam Women's Museum, offer insights into the country's rich heritage.</p><br><br><br>
                    <h2 style="color: white; font-size: 36px;">4. Food</h2><br><hr><br>
                    <img src="restaurant.jpg" width="100%" height="400px">

                    <p>Hanoi is renowned for its delicious street food, which is an integral part of the local culture. Dishes like pho (Vietnamese noodle soup), bun cha (grilled pork with vermicelli), banh mi (Vietnamese sandwich), and egg coffee are just a few examples of the city's culinary delights.</p><br><br><br>
                    <h2 style="color: white; font-size: 36px;">5. Economy and Education</h2><br><hr><br>
                    <img src="capital.jpg" width="100%" height="400px">

                    <p>Hanoi is a major economic center in Vietnam and contributes significantly to the country's GDP. The city's economy is diverse, with industries ranging from manufacturing, technology, and services to tourism.

                        <br><br> Hanoi is home to several prestigious universities and educational institutions, making it an important hub for higher education in Vietnam.
                        
                        <br><br> Hanoi has an extensive public transportation system that includes buses, taxis, and motorbike taxis (xe om). In recent years, the city has been expanding its metro system to ease traffic congestion.</p><br><br><br>
                        <h2 style="color: white; font-size: 36px;">6. Climate</h2><br><hr><br>
                        <img src="climate.jpg" width="100%" height="400px">

                        <p>Hanoi experiences a tropical monsoon climate with four distinct seasons. Summers are hot and humid, while winters can be cool, and it occasionally experiences light snowfall.</p>
                        <div class="social-media">
                            <h2>Follow us on:</h2><br><hr><br>
                            <a href="facebook.com"><i class="ri-facebook-circle-fill"></i></a>
                            <a href="instagram.com"><i class="ri-instagram-line"></i></a>
                            <a href="pinterest.com"><i class="ri-pinterest-line"></i></a>
                        </div> 
                    </div>   
        </div>
        <div class="sideright">
            <h3 class="r-title">More Information</h3>
            <br><br>
            <iframe width="100%" height="300" style="border: 2px solid yellow;" src="https://www.youtube.com/embed/8vYD1fbleEg" title="Hanoi Vietnam Travel Guide: 19 BEST Things To Do In Hanoi" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe><br><br>
            <img src="advertisment.jpg" width="100%" height="500px" ><br><br>
            <img src="second.jpg" width="100%" height="500px"><br><br>
            <img src="thirth.png" width="100%" height="500px">
        </div>
    </div>
    <div class="footer">
        <p>2023 Copyright. All rights reserved</p>
    </div>
</body>
</html>
