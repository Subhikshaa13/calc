# Design of a Standard Calculator

## AIM:

To design a web application for a standard calculator.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
<! DOCTYPE html>  
    <html>  
        <head>  
        <meta charset="utf-8">  
        <title>  
             Calculator using HTML Example  
        </title>  
        <link href="https://fonts.googleapis.com/css2?family=Cookie&display=swap" rel="stylesheet">  
        <!-- CSS property to create interactive  
            calculator interface -->  
        <style>  
            * {  
      box-sizing: border-box;  
      font-family: 'Roboto', sans-serif;  
    }  
    body {  
      background: white;  
    }  
    .container {  
      width: auto;  
      margin: 20px;  
      color:black;  
    }  
    .calc-body {  
      width: 275px;  
      margin: auto;  
      min-height: 400px;  
      border: solid 1px #3A4655;  
      box-shadow: 0 8px 50px -7px black;  
    }  
    .calc-screen {  
      background: #3A4655;  
      width: 100%;  
      height: 150px;  
      padding: 20px;  
    }  
    .calc-operation {  
      text-align: right;  
      color: #727B86;  
      font-size: 21px;  
      padding-bottom: 10px;  
      border-bottom: dotted 1px;  
    }  
    .calc-typed {  
      margin-top: 20px;  
      font-size: 45px;  
      text-align: right;  
      color: #fff;  
    }  
    .calc-button-row {  
      width: 100%;  
      background: #3C4857;  
    }  
    .button {  
      width: 25%;  
      background: #425062;  
      color: #fff;  
      padding: 20px;  
      display: inline-block;  
      font-size: 25px;  
      text-align: center;  
      vertical-align: middle;  
      margin-right: -4px;  
      border-right: solid 2px #3C4857;  
      border-bottom: solid 2px #3C4857;  
      transition: all 0.2s ease-in-out;  
    }  
    .button.l {  
      color: #AEB3BA;  
      background: #404D5E;  
    }  
    .button.c {  
      color: #D95D4E;  
      background: #404D5E;  
    }  
    .button:hover {  
      background: #E0B612;  
      transform: rotate(5deg);  
    }  
    .button.c:hover {  
      background: #E0B612;  
      color: #fff;  
    }  
    .button.l:hover {  
      background: #E0B612;  
      color: #fff;  
    }  
    .blink-me {  
      color: #E0B612;  
    }  
    html {  
      height: 100vh;  
      display: flex;  
      align-items: center;  
      justify-content: center;  
      background-color: #2d3436;  
      background-image: linear-gradient(315deg, #2d3436 0%, #000000 74%);  
      font-family: 'Cookie', cursive;  
    }  
    .title:hover {  
      background: #E0B612;  
      color: #fff;  
    }  
    .title {  
    margin-bottom: 10px;  
    padding: 5px 0;  
    font-size: 40px;  
    font-weight: bold;  
    text-align: center;  
    color: #AEB3BA;  
    font-family: 'Cookie', cursive;  
    }  
    input[type=button] {  
      width: 60px;  
      height: 60px;  
      float: left;  
      padding: 0;  
      margin: 5px;  
      box-sizing: border-box;  
      background: #ecedef;  
      border: none;  
      font-size: 30px;  
      line-height: 30px;  
      border-radius: 50%;  
      font-weight: 700;  
      color: #5E5858;  
      cursor: pointer;    
    }  
    input[type=text] {  
      width: 270px;  
      height: 60px;  
      float: left;  
      padding: 0;  
      box-sizing: border-box;  
      border: none;  
      background: none;  
      color: red;  
      text-align: right;  
      font-weight: 700;  
      font-size: 60px;  
      line-height: 60px;  
      margin: 0 25px;  
      }  
    .calculator {  
      background-color: #c0c0c0;  
      box-shadow: 0px 0px 0px 10px #666;  
      border: 5px solid black;  
      border-radius: 10px;  
    }     
    </style>  
    </head>  
    <body>  
        <div class="container">  
      <div class="calc-body">  
        <div class="calc-screen">  
          <div class="calc-operation"> 25 + 10 = </div>  
          <div class="calc-typed"> 35 <span class="blink-me"> _ </span> </div>  
        </div>  
        <div class="calc-button-row">  
          <div class="button c"> C </div>  
          <div class="button l"> ? </div>  
          <div class="button l"> % </div>  
          <div class="button l"> / </div>  
        </div>  
        <div class="calc-button-row">  
          <div class="button"> 7 </div>  
          <div class="button"> 8 </div>  
          <div class="button"> 9 </div>  
          <div class="button l"> x </div>  
        </div>  
        <div class="calc-button-row">  
          <div class="button"> 4 </div>  
          <div class="button"> 5 </div>  
          <div class="button"> 6 </div>  
          <div class="button l"> ? </div>  
        </div>  
        <div class="calc-button-row">  
          <div class="button"> 1 </div>  
          <div class="button"> 2 </div>  
          <div class="button"> 3 </div>  
          <div class="button l"> + </div>  
        </div>  
        <div class="calc-button-row">  
          <div class="button"> . </div>  
          <div class="button"> 0 </div>  
          <div class="button">  
            < </div>  
              <div class="button l"> = </div>  
          </div>  
        </div>  
      </div>  
    </body>  
    </html>

## OUTPUT:
![calc](https://user-images.githubusercontent.com/118787344/214761479-33458e5c-f00e-4a50-8907-722b5c938991.png)


## HTML VALIDATOR:
![Screenshot (40)](https://user-images.githubusercontent.com/118787344/214761766-314ca31c-9672-4d85-9dfa-7b76b459e2fa.png)


## RESULT:
Simple calculator is executing successfully.

