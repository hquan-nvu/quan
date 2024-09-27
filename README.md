# quan
using Microsoft.AspNetCore.Components.Routing;
using System.Reflection.Metadata;
using System.Reflection.PortableExecutable;
using System;

namespace WebApplication1
{
    public class WeatherForecast
    {
        public DateOnly Date { get; set; }

        public int TemperatureC { get; set; }

        public int TemperatureF => 32 + (int)(TemperatureC / 0.5556);

        public string? Summary { get; set; }
    }
}
< !DOCTYPE html >
< html >
< head >
    < title > Responsive Transparent Login Form Using HTML & CSS</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css" integrity="sha512-iBBXm8fW90+nuLcSKlbmrPcLa0OT92xO1BIsZ+ywDWZCvqsWgccV3gFoRBv0z+8dLJgyAHIhR35VZc2oM/gI1w==" crossorigin="anonymous" />
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.7.2/css/all.css"
        integrity="sha384-fnmOCqbTlWIlj8LyTjo7mOUStjsKC4pOpQbqyi7RrhN7udi9RwhKkMHpvLbHG9Sr" crossorigin="anonymous" />
    <link href="https://fonts.googleapis.com/css?family=Dosis" rel="stylesheet" />
    <link rel="stylesheet" href="style.css">
    
</head>
<body>
   
    <div nav="nav.html"></div>
    <script type="text/javascript" src="main.js"></script>
<script>
function includeHTML() {
  var z, i, elmnt, file, xhttp;
/*loop through a collection of all HTML elements:*/
z = document.getElementsByTagName("*");
for (i = 0; i < z.length; i++)
{
    elmnt = z[i];
    /*search for elements with a certain atrribute:*/
    file = elmnt.getAttribute("nav");
    if (file)
    {
        /*make an HTTP request using the attribute value as the file name:*/
        xhttp = new XMLHttpRequest();
        xhttp.onreadystatechange = function() {
            if (this.readyState == 4)
            {
                if (this.status == 200) { elmnt.innerHTML = this.responseText; }
                if (this.status == 404) { elmnt.innerHTML = "Page not found."; }
                /*remove the attribute, and call this function once more:*/
                elmnt.removeAttribute("nav");
                includeHTML();
            }
        }
        xhttp.open("GET", file, true);
        xhttp.send();
        /*exit the function:*/
        return;
    }
}
};
</ script >

< div class= "bg-img" >
  < div class= "content" >
    < header > SignUp Form </ header >
     < form action = "https://jagadeeshpj.herokuapp.com/" method = "POST" >
      < div class= "field" >
        < span class= "fa fa-user" ></ span >
        < input type = "text" required placeholder = "Email or Phone" >
      </ div >
      < div class= "field space" >
        < span class= "fa fa-lock" ></ span >
        < input type = "password" class= "pass-key" required placeholder = "Password" >
        < span class= "show" > SHOW </ span >
      </ div >
      < div class= "field space" >
        < span class= "fa fa-lock" ></ span >
        < input type = "re-password" class= "pass-key" required placeholder = "Re-Password" >
        < span class= "show" > SHOW </ span >
      </ div >
      < div class= "pass" >
        < a href = "#" ></ a >
      </ div >
      < br >





      < div class= "field" >
        < input type = "submit" value = "LOGIN" >
      </ div >
    </ form >
    < div class= "login" > Or SignUp with</div>
    <div class= "links" >
      < div class= "facebook" >
        < i class= "fab fa-facebook-f" >< span > Facebook </ span ></ i >
      </ div >
      < div class= "instagram" >
        < i class= "fab fa-instagram" >< span > Instagram </ span ></ i >
      </ div >
    </ div >
    < div class= "signup" > Already have an account?
      <a href="index.html">Login</a>
    </div>
  </div>
</div>







<script>
includeHTML();
</ script >
< script src = "https://code.jquery.com/jquery-1.10.2.js" ></ script >





< footer id = "main-footer" >
    < div class= "footer-content container" >
        < p >
            Copyright & copy; 2021 All Rights Reserved
        </p>
        <div class= "social" >
            < a href = "https://github.com/jagadeeshpj" target = "__blank"  style = "color: #fff;" >
                < i class= "fab fa-github" ></ i >
            </ a >

            < a href = "https://www.linkedin.com/in/p-jagadeesh-22923b18b/" target = "__blank"  style = "color: #fff;" >
                < i class= "fab fa-linkedin" ></ i >
            </ a >


            < a href = "https://www.instagram.com/jagadeesh2001/" target = "__blank"  style = "color: #fff;" >
                < i class= "fab fa-instagram" ></ i >
            </ a >

            < a href = "https://www.facebook.com/jagadeesh.PJ.13/" target = "__blank"  style = "color: #fff;" >
                < i class= "fab fa-facebook" ></ i >
            </ a >

        </ div >
    </ div >
</ footer >

</ body >
</ html >
