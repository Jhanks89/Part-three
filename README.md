<html lang="en"> <head> <meta charset="UTF-8"> <meta http-equiv="X-UA-Compatible" content="IE=edge"> <meta name="viewport" content="width=device-width,initial-scale=1"> <meta name="description" content="Maximum JavaScript Homework for voracious people wishing to explore learning."> <link rel="apple-touch-icon" sizes="180x180" href="/favicon/apple-touch-icon.png"> <link rel="icon" type="image/png" sizes="32x32" href="/favicon/favicon-32x32.png"> <link rel="icon" type="image/png" sizes="16x16" href="/favicon/favicon-16x16.png"> <link rel="manifest" href="/favicon/site.webmanifest"> <link rel="mask-icon" href="/favicon/safari-pinned-tab.svg" color="#5bbad5"> <meta name="msapplication-TileColor" content="#da532c"> <meta name="theme-color" content="#ffffff"> <link rel="stylesheet" href="./assets/app.css"> <title> Homework 5.3 | CNIT 133 </title> </head> <body> <div class="container"> <h1>CNIT 133 Homework</h1> </div> <div id="navbar" class="navbar"> <div class="dropdown"> <a class="button" id="1" href="index.html">⚓️</a></div> <h2>Homework 5</h2> <div class="parts button-row"> <a class="button" href="/hw5.1.html">Part 1</a><a class="button" href="/hw5.2.html">Part 2</a><a class="button" href="/hw5.3.html">Part 3</a> </div> <h3>Part 3: The State of the State</h3> <div class="row"> <div class="one-half column"> <form name="myform"> <label for="astate">Enter a state name or abbreviation:</label> <textarea class="u-full-width" id="astate" name="astate" placeholder="Alaska..."></textarea><br> <span class="button-row"> <input type="button" class="button-primary" onclick="process()" value="State Info"> <input type="reset" value="Reset" id="reset"> </span> </form> </div> <div class="one-half column"> <br> <div id="results"></div> </div> <script>const process=()=>{let e=[["AL","Alabama","Montgomery",4887871],["AK","Alaska","Juneau",737438],["AZ","Arizona","Phoenix",7171646],["AR","Arkansas","Little Rock",3010825],["CA","California","Sacramento",39557045],["CO","Colorado","Denver",5694564]],t="We're so sorry, but we couldn't parse your state name. Please try again using only the state's full name or the state's two letter abbreviation. We can currently only parse the first six state names, and only single state names, so just one at a time, please.",a=document.forms.myform.elements.astate.value.replace(/\s+/g,"").toUpperCase();e.forEach(((e,n)=>{a!=e[0]&&a!=e[1].toUpperCase()||(t=n)})),isNaN(t)?document.getElementById("results").innerHTML=t:document.getElementById("results").innerHTML=`Thanks for your inquiry, here is the information you requested:  <br> State abbr = ${e[t][0]} <br> State Name = ${e[t][1]}  <br> Capital = ${e[t][2]}  <br> Population = ${e[t][3].toLocaleString()}`};document.getElementById("reset").addEventListener("click",(()=>{document.getElementById("results").textContent=""}))</script> </div> <br> <br> <script src="/assets/app.bundle.js"></script> <footer class="footer"> <a href="https://github.com/willpuckett/cnit133">🔧</a> | <a href="https://validator.w3.org/check?uri=referer">HTML</a> | <a href="https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fmootrpootr.com%2F/%2Fhw5.3.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en">CSS</a> </footer> </div></body> </html>
