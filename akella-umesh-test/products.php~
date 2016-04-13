<!DOCTYPE html>

<html>
<head>
<title>Bravomedia</title>
<meta name="viewport" content="width=device-width,height=device-height,initial-scale=1">
<link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
<div class="main">
<div class="head">

<div class="logo">
<img src="images/bravomedia_black.png">
</div>

<div class="hm">
<ul>
<li><a href="index.php">Home</a> |</li>
<li><a href="products.php">Products</a> | </li>
</ul>
</div>
</div>

<div class= "body">
<?php

$array=array(parse_ini_file("db.conf"));
$dbhost = $array[0]['IP'];
$port = $array[0]['Port'];
$data = $array[0]['DBname'];
$userid = $array[0]['Username'];
$pwd = $array[0]['Password'];

$con=mysqli_connect($dbhost,$userid,$pwd , $data, $port) ;
$result = mysqli_query($con,"SELECT * FROM products"); 
echo "<table>
<tr>


</tr>";


while($row = mysqli_fetch_array($result))
{echo "<tr>";
  echo "<td>" . "<img src=images/" . $row['image'] ." >" . "</td>";
 echo "</tr>";
  }echo "</table>";


?>


</div>
<div class="footer">
<div class="footleft">
<img src="images/bravomedia_white.png">
</div>

<div class="footright">

Copyright © 2016 by My Company.All rights reserved. Powered by Yii Framework.
</div>
</div>


</div>
</body>
</html>
