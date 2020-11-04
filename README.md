<html>
<head>

<script>
know = {

"Hello" : "&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp  Hi there!",
"hello" : "&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp  Hi there!",
"HELLO" : "&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp  Hi there!",
"Who are you?" : "&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp I am Shashank's Assistant",
"How are you?" : "&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp I am Fine",
"How old are you?" : "&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp I am infinity in age"




};

function talk() {
var user = document.getElementById("userBox").value;
document.getElementById("userBox").value= "";
document.getElementById("chatLog").innerHTML += user+"<br>";

if (user in know) {
document.getElementById("chatLog").innerHTML += know[user] + "<br>";
} else 

{
document.getElementById("chatLog").innerHTML += "I don't understand... <br>";
}
}





</script>



</head>


<body>

<p id="chatLog"> - - ChatBot By Crazy Codes - - <br> </p>

<input id="userBox" type="text" onkeydown="if(event.keyCode == 13) {talk()}">


</body>



</html>
