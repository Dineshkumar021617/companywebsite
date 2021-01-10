# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Silicon Private Limited</title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel = "icon" href ="{% static 'img/titleicon.png' %}" type = "image/x-icon"> 
              
</head>

<body>
    <div class="container">
    <div class="banner">
        Silicon Private Limited.
    </div>
    <div class="menu">
        <div class="menuitem"><a href="/home">Home</a></div> 
        <div class="menuitem"><a href="/products">Products</a></div> 
        <div class="menuitem"><a>People</a></div>
        <div class="menuitem"><a>Contact Us</a></div> 
    </div><div class="content">
    {% block content %}    
    {% endblock  %}
    </div>
    <div class="footer">
        Copyright © 2020 Silicon Private Limited, Developed by Obed Otto.
    </div>
    </div>
</body>

</html>
```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="homecontent">    
    <h1>About Us</h1>
    <img src="/static/img/building2.jpeg" alt="Building">
    <div class="contenttext">
    Silicon Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications. Some of Silicon's core technologies and products include:
    <ul>
        <li>Memory Chips</li>
        <li>SATA HDD</li>
        <li>SATA SSD </li>
        <li>Broadband Modems</li>
        <li>Wifi Devices</li>
        <li>Switching Devices</li>
        <li>Optical Sensors</li>
    </ul> 
    </div>
    </div>
{% endblock  %}
```
### products.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="productcontent">    
    <h1>Our Premium Products</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c1.jpg" alt="product image">
            </div>
            <div class="itemname">4GB DDRA4 laptop memory</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c2.jpg"  alt="product image">
            </div>
            <div class="itemname">1TB Laptop HDD</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c3.jpg"  alt="product image">
            </div>
            <div class="itemname">1TB 665p Series M.2 2280 PCIe NVMe 3.0 x4 3D3, QLC Internal Solid State Drive (SSD)</div>
            <div class="itemprice">Price: Rs.12000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c4.jpg"  alt="product image">
            </div>
            <div class="itemname">2TB 3D NAND NVMe PCIe Internal SSD</div>
            <div class="itemprice">Price: Rs.38000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c5.jpg"  alt="product image">
            </div>
            <div class="itemname">16GB Single DDR4 2666  PC4-21300 DR x8 SODIMM 260-Pin RAM</div>
            <div class="itemprice">Price: Rs.7000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c6.jpg"  alt="product image">
            </div>
            <div class="itemname">8GB DDR4 modules for notebooks 2666 Laptop Memory</div>
            <div class="itemprice">Price: Rs.10000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c7.jpg"  alt="product image">
            </div>
            <div class="itemname">8GB DDR4-2400 PC4-19200 CL-17 SODIMM RAM</div>
            <div class="itemprice">Price: Rs.2800.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c8.jpg"  alt="product image">
            </div>
            <div class="itemname">Analog to Digital Breakout Board</div>
            <div class="itemprice">Price: Rs.600.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c9.jpg"  alt="product image">
            </div>
            <div class="itemname">ATmega32 Microcontroller</div>
            <div class="itemprice">Price: Rs.100.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c10.jpg"  alt="product image">
            </div>
            <div class="itemname">PIC Development Board ZIF Socket with On Board PIC16F877A MAX232</div>
            <div class="itemprice">Price: Rs.900.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c11.jpg"  alt="product image">
            </div>
            <div class="itemname">Quick Starter Development Board and AVR USB ISP Programmer Starter Kits</div>
            <div class="itemprice">Price: Rs.1000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c12.jpg"  alt="product image">
            </div>
            <div class="itemname">Infrared (IR) Proximity or Obstacle Detecting Sensor Module</div>
            <div class="itemprice">Price: Rs.100.00 </div>
        </div>
    </div>
    </div>
{% endblock  %}
```
### people.html:
```
{% extends "website/base.html" %}

{% block content %}
    <div class="peoplecontent">
        <div>
            <div class="peopleimg">
                <img src="http://lms.ai.saveetha.ac.in/pluginfile.php/15229/user/icon/boost/f1?rev=12005" alt="people image">
            </div>
            <div class="peopledetails">
                <h3>Aakash.V.P</h3>
                <h3>B.Tech</h3>
            </div>
        </div>
        <div>
            <div class="peopleimg">
                <img src="http://lms.ai.saveetha.ac.in/pluginfile.php/16200/user/icon/boost/f1?rev=11960" alt="people image">
            </div>
            <div class="peopledetails">
                <h3>Aishree</h3>
                <h3>B.Tech</h3>
            </div>
        </div>
        <div>
            <div class="peopleimg">
                <img src="http://lms.ai.saveetha.ac.in/pluginfile.php/16292/user/icon/boost/f1?rev=42288" alt="people image">
            </div>
            <div class="peopledetails">
                <h3>Dineshkumar.S</h3>
                <h3>B.Tech</h3>
            </div>
        </div>
        <div>
            <div class="peopleimg">
                <img src="http://lms.ai.saveetha.ac.in/pluginfile.php/16450/user/icon/boost/f1?rev=12223" alt="people image">
            </div>
            <div class="peopledetails">
                <h3>Ashwin.A.O</h3>
                <h3>B.Tech</h3>
            </div>
        </div>
         <div>
            <div class="peopleimg">
                <img src="http://lms.ai.saveetha.ac.in/pluginfile.php/15234/user/icon/boost/f1?rev=12123" alt="people image">
            </div>
            <div class="peopledetails">
                <h3>Graham Stanes</h3>
                <h3>B.Tech</h3>
            </div>
        </div>
         <div>
            <div class="peopleimg">
                <img src="http://lms.ai.saveetha.ac.in/pluginfile.php/16735/user/icon/boost/f1?rev=12353" alt="people image">
            </div>
            <div class="peopledetails">
                <h3>Sumyuktha Rani</h3>
                <h3>B.Tech</h3>
            </div>
        </div>
    </div>
{% endblock  %}
```
### contactus.html:
```
{% extends "website/base.html" %}

{% block content %}
    <div>
        <h2>CONTACT US</h2>
        <h3 id="h3">We're are glad to help you!</h3>
        <div>
            <form class="complaints" action="/test" method="POST">
                <textarea placeholder="Your name" rows="1" cols="50" name="name" id="name"></textarea><br>  
                <textarea type="text" placeholder="E-mail" rows="1" cols="50" name="email" id="email"></textarea><br>
                <textarea name="message" id="message" rows="8" cols="50" placeholder="Message"></textarea><br>
                <button type="submit" name="submit" id="submit">Sumbit</button>
            </form>
            <div class="contactus">
                <div>
                    <img class="address" src="https://us.123rf.com/450wm/lililia/lililia1711/lililia171100435/90687353-vector-flat-icon-of-geolocation-on-black-background.jpg?ver=6">
                    <a>#140,BK nagar,Adyar,Chennai-600020</a>
                </div>
                <div>
                    <img class="address" src="https://i.pinimg.com/474x/47/ee/93/47ee9334101d8d875da877bec5f46f47.jpg">
                    <a>044-2474 8291</a>
                </div>
            </div>
        </div>
    </div>
{% endblock %}
``` 
## OUTPUT:
![output](./static/img/output1.png)
![output](./static/img/output2.png)
![output](./static/img/output3.png)
![output](./static/img/output4.png)


## CODE VALIDATION REPORT:
![output](./static/img/report1.png)
![output](./static/img/report2.png)
![output](./static/img/report3.png)
![output](./static/img/report4.png)
## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://dineshkumars.student.saveetha.in:8000/. HTML code is validated.