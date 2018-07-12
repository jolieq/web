<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
    box-sizing: border-box;
}

body {
  margin: 10px;
  max-width:2000px;
}

.header {
    background-color: #f1f1f2;
    padding-top: 15px;
    text-align: center;
    color: black;
    font: 80px big caslon;
    max-width:2000px;
}

.header2 {
	text-align: center;
    color: black;
    font: 45px big caslon;
    padding-bottom: 0px;
}


.header3{
	text-align: center;
    color: black;
    font: 20px big caslon;
    padding-top: 0px;

}

/* Style the top navigation bar */
.topnav {
    overflow: hidden;
    background-color: #f1f1f2;
    max-width:2000px;
}

/* Style the topnav links */
.topnav a.two {
    float: left;
    display: block;
    color: black;
    text-align: center;
    padding: 10px 16px;
    text-decoration: none;
    font-size: 15px;
    margin-right: 10px;
    position: relative;
    max-width:2000px;
}



a.two:before {
  content: "";
  position: absolute;
  width: 100%;
  height: 2px;
  bottom: 0px;
  left: 0px;
  background-color: black;
  visibility: invisible;
  -webkit-transform: scaleX(0);
  transform: scaleX(0);
  -webkit-transition: all 0.3s ease-in-out 0s;
  transition: all 0.3s ease-in-out 0s;
}

a.two:hover:before {
  visibility: visible;
  -webkit-transform: scaleX(1);
  transform: scaleX(1);
}

.topnav-right{
	float: right;

}

.QMM {
	color: black;
    float: left;
    padding: 10px 16px;
    display: block;
    position: relative;
    width: 260px;
    text-align: center;
    font-size: 15px;
    
}

.QMM:hover {
	visibility: invisible;
    font-size:0px;
    padding: 10px 16px;
    border: 2px solid black;
    width: 240px;
    height: 39px;
    transition: .4s;

}

.QMMtext {
	text-decoration: none;
    font-size:0;
}

.QMM:hover .QMMtext.right{
    color: black;
    font-size: 15px;
    transition: .4s;
    float: right;
    overflow: hidden;
    white-space: nowrap;
    position: relative;
    box-sizing: border-box;
}

.QMM:hover .QMMtext.left{
    color: black;
    font-size: 15px;
    padding-bottom: 20px;
    transition: .4s;
    float: left;
    overflow: hidden;
    white-space: nowrap;
    position: relative;
    box-sizing: border-box;
}

.QMM:hover .QMMtext.right:hover{
	text-decoration: underline;
    color: black;
    font-size: 15px;
    transition: .4s;
    float: right;
}

.QMM:hover .QMMtext.left:hover{
	text-decoration: underline;
    color: black;
    font-size: 15px;
    transition: .4s;
    float: left;
}


/* Create three unequal columns that floats next to each other */
.column {
	margin-top: 10px;
    float: left;
    padding-top: 20px;
    padding-bottom: 20px;
    padding-left: 30px;
    padding-right: 40px;
    max-width: 2000px;

}

/* Left and right column */
.column.side {
    width: 48%; 
    margin-left: 15px;
}

.column.side:hover {
	background-color: #edf1f7;
   
}

/* Middle column */
.column.middle {
	padding-left: 30px;
    width: 50%;
 
}

.column.middle:hover {
	padding-left: 30px;
	background-color: #edf1f7;
}

.column.center {
	width: 50%;
}

.column.center:hover {
    text-decoration: underline;
}

/* Clear floats after the columns */
.row:after {
    content: "";
    display: table;
    clear: both;
}

/* Responsive layout - makes the three columns stack on top of each other instead of next to each other */
@media screen and (max-width: 400px) {
    .column.side, .column.middle {
        width: 100%;
    }
}

p.border {
	border: 1px solid black;
    padding: 3px 5px;
    border-radius: 5px; 
}

.button.one:link, .button.one:visited{
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    -webkit-transition-duration: 0.4s; /* Safari */
    transition-duration: 0.4s;
    cursor: pointer;
	width: 100%;
    background-color: white;
    color: black;
    border: 2px solid #555555;
}

.button.one:hover, .button.one:active {
    background-color: #555555;
    color: white;
   
}

.button.two{
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    margin-bottom: 13px;
    padding: 2px;
    -webkit-transition-duration: 0.4s; /* Safari */
    transition-duration: 0.4s;
    /* cursor: pointer; */
	width: 100%;
    background-color: white;
    color: black;
    border: 2px solid #555555;
    position: relative;
    
}

.button.two:hover {
	text-decoration: none;
    background-color: #555555;
    color: white;
    transition-duration: 0.4s;
    text-align: left;
    padding-left: 10px;
    font-size: 30px;
    font-color: white;
   
}

.tabs{
	opacity: 0;
    display: inline-block;
    float: right;
	text-align: right;
    padding-right: 10px;
    font-size: 0px;
    
}

.button:hover .tabs{
	opacity: 1;
	text-decoration: none;
    text-align: middle;
    color: white;
    float: right;
    padding-right: 10px;
    padding-top: 13px;
    font-size: 18px;
    word-spacing: 20px;

}

a.white{
	color: white;
    text-decoration: none;
}

a.white:hover{
	text-decoration: underline;
    color: white;
}



.footer {
    position: static;
    left: 0;
    bottom: 0;
    width: 100%;
    background-color: white;
    text-align: right;
    padding-right: 15px;
}


</style>
</head>
<body>

<div class="header">
  <p>Tech Support</p>
</div>

<div class="topnav">
   <a class="two" href="http://sp.ksec.com/TechSupport/Lists/Calendar/calendar.aspx" class="topnav a">Calendar</a>
   <a class="two" href="http://sp.ksec.com/QualityAssurance/Lists/Calendar/calendar.aspx" class="topnav a">Safety</a>
   <div class="two QMM"> QMM
   <a class="QMMtext left" href="#"> Important Notice </a>
   <a class="QMMtext right" href="#"> Tech Info </a>
   </div> 
   <div class="topnav-right">
<a class="two" href="http://sp.ksec.com/SitePages/Home.aspx" class="topnav a">Kokusai Home</a>
</div>
</div>


<div class="row">
  <div class="column side">
<p><a class="one button" href="http://sp.ksec.com/QualityAssurance/Working%20Documents/Forms/AllItems.aspx">ECN</a></p>
    
  	<p><a class="one button" href="http://sp.ksec.com/TechSupport/Fans/Forms/AllItems.aspx">FANS</a></p>
    
    <div class="button shift two">PARTS<div class="tabs">
    <a class="white" href="#">200mm</a>
    <a class="white" href="#">300mm</a>
    </div>
    </div>
    
 <p><a class="one button" href="http://sp.ksec.com/QualityAssurance/Temporary/Forms/AllItems.aspx">TS/TOOLS</a></p>
  </div>
  
  <div class="column middle">
    <p><a class="one button" href="#">CALIBRATION</a></p>
 	<p><a class="one button" href="#">MEETING MINUTES</a></p>
    <p><a class="one button" href="#">INSTALL BASE</a></p>
    <p><a class="one button" href="#">SOFTWARE</a></p>
    <p><a class="one button" href="#">INSTALL</a></p>
    <p><a class="one button" href="#">SERVICE</a></p>
    
    <div class="button shift two">ESCALATIONS<div class="tabs">
    <a class="white" href="#">Escalations</a>
    <a class="white" href="#">Post-Mortem</a>
    </div>
    </div>
	</div>

    
    </div>
   

  
<div class="footer">
<p>Jolie Qiu</p>
</div>
  
</body>
</html>




