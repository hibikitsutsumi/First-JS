<!DOCTYPE html>
<html>
<head>
	<title>JS</title>
<link rel="stylesheet" type="text/css" href="style.css">
		

</head>
<body>
	
	<h1> fruit game</h1>
	<input type="button" onclick="game();" name="ok" value="start">
    <p> Based on your favorite fruit we will jugde you! win or not</p>
<p id="demo">Result will be here</p>
<script type="text/javascript" src="main.js"></script><!-- this line is really important-->
</body>
</html>
--------------------------------------------------------
function game(){
let fruit = "apple";
let userInput = prompt("What is your favorite fruit?");
let info = document.getElementById("demo")

if( userInput.toLowerCase() === fruit){
	info.innerHTML = ("you won the apple prize");
}else{
	info.innerHTML = ("you lost");
}
}
----------------------------------------------------------
body{
	text-align: center;
}

p{
	color: darkgrey;
}

h1{
	margin-top: 20%;
	
}

#demo{
	color: #FF6347;
	font-size: 2em;
	background-color: #FFBF47;
	padding: 5px;
	border: 1px dashed black;
	display: inline;
}
