
</style>
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {box-sizing: border-box}

/* Set height of body and the document to 100% */
body, html {
  height: 100%;
  margin: 0;
  font-family: Arial;
}

h1{
text-align:center;
}
a
{
color:black;
}
/* Style tab links */
.tablink {
  background-color: #555;
  color: white;
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 14px 16px;
  font-size: 17px;
  width: 25%;
}

.tablink:hover {
  background-color: #777;
}

/* Style the tab content (and add height:100% for full page content) */
.tabcontent {
  color: white;
  display: none;
  padding: 100px 20px;
  height: 100%;
}

#Home {background-color: red;}
#News {background-color: green;}
#Contact {background-color: blue;}
#About {background-color: orange;}
</style>
</head>
<body>

<button class="tablink" onclick="openPage('Home', this, 'red')">Home</button>
<button class="tablink" onclick="openPage('Software', this, 'violet')">Software</button>
<button class="tablink" onclick="openPage('Contact', this, 'blue')">Contact</button>
<button class="tablink" onclick="openPage('About', this, 'orange')">About</button>

<div id="Home" class="tabcontent">
  <h3>Home</h3>
  <p>



Hi! I am harshavardhana.
<br>
Go to <a href="https://codepen.io">codepen</a> and search harshavardhana-holla-gmail-com


  </div>
</div></p>
</div>


<div id="Contact" class="tabcontent">
  <h3>Contact</h3>
  <p>Hello Everyone Email<a href="mailto:harshavardhana.holla@gmail.com"> <mark>me!</mark></a></p>
</div>
<div id="Software" class="tabcontent" style="background-color:violet;;">
  <h3>Software</h3>
  <p>Here are some links for the software I built!</p>
  <br>
  <a href="https://github.com/harshavardhana505">View source code of software on github</a>
</div>

<div id="About" class="tabcontent">
  <h3>About</h3>
  <p>I am Harshavardhana Building simple software</p>
</div>

<script>
function openPage(pageName,elmnt,color) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablink");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].style.backgroundColor = "";
  }
  document.getElementById(pageName).style.display = "block";
  elmnt.style.backgroundColor = color;
}

// Get the element with id="defaultOpen" and click on it
document.getElementById("defaultOpen").click();
</script>
   
</body>
</html> 




