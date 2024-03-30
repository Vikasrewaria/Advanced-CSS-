Task 1:- 
Problem statement 
Explain the purpose of using the var() function in CSS. Also you have ccreated two buttons with id named PrimaryBtn and secondaryBtn which should be given background colors using the var() function. The color code for primarycolor is #00b7ff and secondarycolor is #6c757d.
Answer:-
<br>The var() function in css is used to reference and use the value of a custom property (also known as a CSS variable) within your stlesheets. CSS variable are defined usingg the --prefix followed by a variable name.
They allow us to store and refuse values throughot our stylesheet, making it easier to maintain consistency and make global changes.
Purpose of var() function.
1. Reusability: CSS variables allow us to store values that we can rese across our stylesheet. The var() function lets us reference these values whereve needed, reducing redundancy and making our code cleaner.
2. Consistency: By using variables, we can ensure consistent values for color, spacing, fonts, and more throughout our entire design. Changing a variable's value wwill automatically update all instances where the variable is used.
3. Global Changes: If we need to make a design change, we can update the variable;s value once, and the change will be applied to all instances using that variable.
<br>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Task-1</title>
</head>
  <style>
    body{
        margin: 0px;
        padding:0px;
    }
    :root{
        --primarycolor:#00b7ff;
        --secondarycolor:#6c757d;
    }
    button{
        padding: 10px;
        color: white;
        border:none;
    }
    #primaryBtn{
        background-color: var(--primarycolor);
    }
    #secondaryBtn{
        background-color: var(--secondarycolor);
    }
</style>
<body>
        <button id="primaryBtn">Priamry Button </button>
        <button id="secondaryBtn">Secondary Button </button>
</body>
</html>

<br>

Task.2:- 
Problem Statment:- <br>
Crate a 3D cube using the trasform prpeerty of css.
Solution:-  
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Task 2</title>
    <style>
       
         .screen{ 
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
        } 
        .cube{

            height: 200px;
            width: 200px;
            position: relative;
            transform-style:preserve-3d;
            transform: rotateX(20deg) rotateY(30deg);
        }
        .face{
            position:absolute;
            height: 200px;
            width: 200px;
            font-weight: bold;
            background-color:rgba(0, 123, 255, 0.7);
            opacity: 0.8;
            border: 1px solid #666;
       display: flex;
       justify-content: center;
       align-items:center;           
        }
        .front{
            transform: translateZ(100px);
        }
        .right{
            transform: rotateY(90deg) translatez(100px);
        }
        .left{
            transform: rotateY(-90deg) translatez(100px);
        }
        .top{
            transform: rotateX(90deg) translateZ(100px);
        }
        .bottom{
            transform:rotateX(-90deg) translateZ(100px);
        }
        .back {
            transform: rotateY(180deg) translateZ(100px);
        }
    </style>
</head>
<body>
    <div class="screen">
        <div class="cube">
            <div class="face front">Front</div>
            <div class="face back">back</div>
            <div class="face right">Right</div>
            <div class="face left">Left</div>
            <div class="face bottom">Bottom</div>
            <div class="face top">Top</div>
        </div>
    </div>
    
</body>
</html>

Task.3:- 
Problem Statment
Create a simple circlar loader which will rotate continuously to look like a loading screen on a website.

Solution:- <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>loader</title>
    <style>
        .main{
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        .loader{
            height: 200px;
            width: 200px;
            border: 10px solid grey;
            border-radius: 50%;
            border-right-color:blue;
            animation: spin 1s linear infinite;
        }
        @keyframes spin{
            0%{
                transform: rotate(0deg);
            }
            100%{
                transform: rotate(360deg);
            }
        }
    </style>
</head>
<body>
        <div class="main">
            <div class="loader"></div>
        </div>
</body>
</html>

Task.4:-   
Problem Statment
You have to visit the PW skills website (https://pwskills.com/) and have to hide the logo by using the developer tool. This should be done using the css and developer tool only, use of javascript is prohibited.
Answer:- ![Task-4](https://github.com/Vikasrewaria/Advanced-CSS-/assets/144261695/bd93c6f6-f53a-48ba-9fba-6ce53e0e8994)



Task.5 :- 
Prolem Statment
You have to visit the PW skills website ad have to change the content of the "login / Registration" button to "connect with us" using the developer tool. This should be done using the elements of developers tools only, use of javascript is prohibted.

Solution:- ![Task-5](https://github.com/Vikasrewaria/Advanced-CSS-/assets/144261695/16723781-6a95-4909-83af-3b6f23b64f4c)



