Fully working PHP/AJAX contact form script is available in the pro version of the template.
You can buy it from: https://bootstrapmade.com/personal-free-resume-bootstrap-template/


<?php
    $name= $_POST['name'];
    $visitor_email = $_POST['email']
    $message = $_POST['message']


    $email_form = 'subhashjha15701@gmail.com';
     
    $email_subject = "New Form Submission";

    $email_body = "User Name: $name.\n".
                    "User Email:$visitor_email.\n".
                        "User Messsage : $message.\n";

    
    $to = "subashjha18@hotmail.com";

    $headers = "From: $email_from  \r\n";

    $headers = "Reply-To: $visitor_email \r\n";

    mail($to,$email_subject,$email_body,$headers);

    header("Location: index.html")


?>