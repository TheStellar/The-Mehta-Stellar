<P aligne="Left"> <img SRC="Pictures/Logo.jpg" WIDTH="200" HEIGHT="120"></P>
<h1>The Mehta Stellar</h1>
Welcome to the Professional Automobile Consultation and Assessment Services
<p>Hi Guys Welcome to the world of Professional Consultation in the field of Automobile Sales and Service Operations.
I am An Automobile Professonal with 12 + Years of experiance in the Field of Automobile Manufacturing, Field Service, 
Sales and Assessments related to Automobiles Skill sets as Per ASDC.
I welcomes you all to the world of new learning and opportunities.</p>
<form action="mail.php" method="POST">
<p>Name</p> <input type="text" name="name">
<p>Email</p> <input type="text" name="email">
<p>Phone</p> <input type="text" name="phone">
<p>Dropdown Box</p>
<select name="dropdown" size="1">
<option value="Area">Himachal</option>
<option value="Area">Panchkulla</option>
<option value="Area">Chandigarh</option>
<option value="Area">others</option>
</select>
<br />
<p>Message</p><textarea name="message" rows="6" cols="25"></textarea><br />
<input type="submit" value="Send"><input type="reset" value="Clear">
</form>
<?php
$name = $_POST['name'];
$email = $_POST['email'];
$dropdown = $POST['dropdown'];
$message = $_POST['message'];
$formcontent="From: $name \n Message: $message";
$recipient = "jai.mehta85@outlook.com";
$subject = "Contact Form";
$mailheader = "From: $email \r\n";
mail($recipient, $subject, $formcontent, $mailheader) or die("Error!");
echo "Thank You!";
?>
