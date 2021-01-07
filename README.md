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
    <title>Copper Private Limited</title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel = "icon" href ="{% static 'img/titleicon.png' %}" type = "image/x-icon"> 
              
</head>

<body>
    <div class="container">
    <div class="banner">
        Copper Private Limited.
    </div>
    <div class="menu">
        <div class="menuitem"><a href="/home">Home</a></div> 
        <div class="menuitem"><a href="/products">Products</a></div> 
        <div class="menuitem"><a href="/people">People</a></div>
        <div class="menuitem"><a href="/contactus">Contact-Us</a></div> 
    </div><div class="content">
    {% block content %}    
    {% endblock  %}
    </div>
    <div class="footer">
        Copyright © 2020 Copper Private Limited, Developed by Gowri.
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
    <img src="/static/img/firstpic.png" alt="Building">
    <div class="contenttext">
        Established in the year 2004, we “Copper Private Limited” have gained immense recognition in the domestic market as a
        leading trader of Ferrous & Non – Ferrous metal Products. Procured from authenticated vendors, these products
        are assured to be at par with the international quality standards.
        <h2>Our range encompasses following products:</h2>
        <ul>
            <li>Forging</li>
            <li>Structural Steels</li>
            <li>Plates </li>
            <li>Pipes & Tubes</li>
            <li>Manifold Blocks</li>
            <li>Alloy Steels</li>
            <li>Bright Bars</li>
            <li>Fittings</li>
            <li>Castings</li>
            <li>Industrial Steels</li>
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
            <img src="/static/img/product1.png" alt="product image">
            </div>
            <div class="itemname">Deoxidised Low Phosphorus(DLP) Copper Tubey</div>
            <div class="itemprice">Price: Rs 550  / Kg </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/product2.png"  alt="product image">
            </div>
            <div class="itemname">Tellurium Copper Rod</div>
            <div class="itemprice">Price: Rs 700 / Kg </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/product3.png"  alt="product image">
            </div>
            <div class="itemname">Tellurium Copper Strip</div>
            <div class="itemprice">Price:Rs 730 / Kg </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/product4.png"  alt="product image">
            </div>
            <div class="itemname">Silver Bearing Copper Strip</div>
            <div class="itemprice">Price:Rs 800 / Kg </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/product5.png"  alt="product image">
            </div>
            <div class="itemname">Deoxidised Low Phosphorus Copper Rod</div>
            <div class="itemprice">Price:Rs 950 / Kg </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/product6.png"  alt="product image">
            </div>
            <div class="itemname">Copper Rod ( Electrolytic Tough Phosphorus)</div>
            <div class="itemprice">Price:Rs 1766 / Kg </div>
        </div>
          <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/product7.png"  alt="product image">
            </div>
            <div class="itemname">Copper Hollow Profiles</div>
            <div class="itemprice">Price:Rs 1233 / Kg </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/product8.png"  alt="product image">
            </div>
            <div class="itemname">Deoxidised High Phosphorus(DHP) Copper Strips</div>
            <div class="itemprice">Price:Rs 550 / Kg </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/product9.png"  alt="product image">
            </div>
            <div class="itemname">Press Components</div>
            <div class="itemprice">Price:Rs 430 / Kg </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/product10.png"  alt="product image">
            </div>
            <div class="itemname">Integral Finned Tubes</div>
            <div class="itemprice">Price:Rs 1970 / Kg </div>
        </div>
          <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/product13.png"  alt="product image">
            </div>
            <div class="itemname">Bare Copper Wire</div>
            <div class="itemprice">Price:Rs 197 / Kg </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/product14.png"  alt="product image">
            </div>
            <div class="itemname">Copper Billet</div>
            <div class="itemprice">Price:Rs 650 </div>
        </div>
    </div>
    </div>
    
{% endblock  %}
```
### people.html
```
{% extends "website/base.html" %}

{% block content %}
<div>
    <h1>Our team</h1>
    <div>
        <div>
            <div>
                <img src="/static/img/peo1.png" alt="people image">
            </div>
            <h2>Shri Aaditkhan</h2>
            <h4>CEO of copper labs </h4>
        </div>
        <div>
            <div>
                <img src="/static/img/peo2.png" alt="people image">
            </div>
            <h2>Andrews</h2>
            <h4>Senior Manager Officer </h4>
        </div>
        <div>
            <div>
                <img src="/static/img/peo3.png" alt="people image">
            </div>
            <h2>Merolin</h2>
            <h4>Chairman of the Copper labs </h4>
        </div>
        <div>
            <div>
                <img src="/static/img/peo4.png" alt="people image">
            </div>
            <h2>Ragunath A.Mashelkar</h2>
            <h4> Chief Financial Officer </h4>
        </div>
        <div>
            <div>
                <img src="/static/img/peo5.png" alt="people image">
            </div>
            <h2>Shri Yogendra P.Trivendi</h2>
            <h4>Marketing Manager </h4>
        </div>
        <div>
            <div>
                <img src="/static/img/peo6.png" alt="people image">
            </div>
            <h2>Prof Deepak C.Jain</h2>
            <h4>Copper Labs' Chief Technology Officer </h4>
        </div>
    </div>
</div>
{% endblock  %}
```
### contactus.html
```
{% extends "website/base.html" %}

{% block content %}
<div>
    <h1>Contact details</h1>
    <div>
        <h2>Contact person:</h2>
            <h4>Vijay Kharti (director)</h4>

        <h2>Address:</h2>
        <h4>Copper Private Limited</h4>
        <h4>No. 1-A, Puliambedu, Numbal,</h4>
        <h4> Off Poonamallee High Road,</h4> 
        <h4>Chennai - 600077,</h4> 
        <h4>Tamil Nadu, India</h4>
        
        <h2>Call us:</h2>
        <h4>080678 54633</h4>
    </div>
    <div>

        <h1>Other contact details</h1>
        <h4>Sales Enquiry</h4>
        <h4> Kavita</h4> 
        <h4>1A puliembedu, Numbal, Off PH Rd,</h4>
        <h4>Chennai - 600077, India</h4>

        <h3>Head Office</h3>
        <h4>Kamal Khatri,</h4>
        <h4>1A Puliembedu, Numbal,</h4> 
        <h4>Off Poonamallee High Road, India</h4>
        
        

        <h3>Branch Office</h3>
        <h4>Vijay Khatri</h4>

        <h3>Head Office</h3>
        <h4>Srinivasan</h4>
        <h4>1A puliembedu, Numbal,</h4>
        <h4> Off PH Rd, Chennai -600077, India</h4>

       </div>
</div>

{% endblock  %}
```

## OUTPUT:
![output](./static/img/output1.png)

![output](./static/img/output2.png)

![output](./static/img/output3.png)

![output](./static/img/output4.png)

![output](./static/img/output5.png)

![output](./static/img/output6.png)

![output](./static/img/output7.png)

![output](./static/img/output8.png)

![output](./static/img/output9.png)

![output](./static/img/output10.png)



## CODE VALIDATION REPORT:
![output](./static/img/val1.png)

![output](./static/img/val2.png)

![output](./static/img/val3.png)

![output](./static/img/val4.png)
## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://gowri.student.saveetha.in:8000/. HTML code is validated.