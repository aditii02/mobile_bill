<html>
<head>
<title>form validation</title>

<script>
function calculate()
{
var z = parseInt(document.getElementById("numcalls").value);
var sum ;
if(z>=100)
{
sum = z*3;

}
else if(z< 100)
{
sum =z*2;
}
alert("bill:" +sum);
alert("OK");
}
</script>
</head>

<body>
<form>
<table align="center">
<style>
table,th,td{ border: 5px solid black; border-collapse: collapse;}
th{text-align:left;}
th,td{padding:10px;}
</style>

<caption>mobile bill</caption>
<tr>
<th>
mobile no:
<input type="text" pattern="[0-9]{10}" title="number should be 10 digits" required/><br>
</th>
</tr>
<tr>
<th>
name:
<input type="text" required/><br>
</th>
</tr>
<tr>
<th>
email:
<input type="email" title="type your email" required/><br>
</th>
</tr>

<tr>
<th>
no of calls:
<input type="text" id="numcalls" pattern="[0-9].{0,4}" title="enter calls" required/><br>
</th>
</tr>
<tr>
<th>
calculate amount:
<input type="button" onclick="calculate()" value="Submit" />



</th>
</tr>
</table>
</form>
</body>
</html>


