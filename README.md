# Ex.08 Design of Interactive Image Gallery
## Date: 16.12.2024

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Image Gallery</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRggGGjq-ecHM-a2rm2ZhKO3wvU2RPz34OWMg&s);
            background-repeat: no-repeat;
            background-size: cover;
        }

        header {
            text-align: center;
            font-size: 32px;
            font-family: Arial, Helvetica, sans-serif;
            color: white;
        }

        div img {
            width: 225px;
            height: 225px;
            cursor: pointer;
            border-radius: 10px;
        }
        .img{
            overflow: hidden;
        }
        div{
            transition: 0.25s;
        }

        div :hover {
            transform: scale(1.1);
            border-radius: 10px;
        }
        
        
        .col1 {
            display: flex;
            gap: 30px;
            margin-top: 30px;
            justify-content: center;
        }
        .col2 {
            display: flex;
            gap: 30px;
            margin-top: 30px;
            justify-content: center;
        }

        

        span {
            color: white;
            position: absolute;
            top: 5%;
            right: 5%;
            font-size: 50px;
            cursor: pointer;
        }
        #dis{
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.8);
            position: fixed;
            top: 0;
            bottom: 0;
            display: none;
            align-items: center;
            justify-content: center;
            z-index: 100;
        }
        #dis img{
            width: 400px;
            height: 400px;
        }
    </style>
    
</head>

<body>
    <header>
        <h1>My Image Gallery</h1>
    </header>
    <section id="dis">
        <img src="dhoni.png" alt="" id="disimg">
        <span class="cls" onclick="closes()">&times;</span>
        
    </section>
    <div class="col1">
        <div class="img">
            <img src="dhoni wc.jpg" onclick="opens(this.src)" id="img1" alt="">
        </div>
        <div class="img">
            <img src="dhonit20.jpg" onclick="opens(this.src)" id="img2" alt="">
        </div>
        <div class="img">
            <img src="dhoni champ.jpg" onclick="opens(this.src)" id="img3" alt="">
        </div>
        <div class="img">
            <img src="vijay.webp" onclick="opens(this.src)" id="img4" alt="">
        </div>
    </div>
    <div class="col2">
        <div class="img">
            <img src="dhoni ipl.jpg" onclick="opens(this.src)" id="img5" alt="">
        </div>
        <div class="img">
            <img src="dhonimace.jpg" onclick="opens(this.src)" id="img6" alt="">
        </div>
        <div class="img">
            <img src="dhoni.png" onclick="opens(this.src)" id="img7" alt="">
        </div>
        <div class="img">
            <img src="mahirat.jpg" onclick="opens(this.src)" id="img8" alt="">
        </div>

    </div>
    

    <script>
        var dis=document.getElementById("dis");
        var disimg=document.getElementById("disimg");
        function opens(image){
            dis.style.display="flex";
            disimg.src=image;
        }
        function closes(){
            dis.style.display="none";

        }
    </script>
</body>

</html>
```
## OUTPUT:
![text](<Screenshot 2024-12-16 182839.png>) 
![text](<Screenshot 2024-12-16 182848.png>) 
![text](<Screenshot 2024-12-16 182856.png>) 
![text](<Screenshot 2024-12-16 182907.png>) 
![text](<Screenshot 2024-12-16 182913.png>)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
