# validateEmail
simple jQuery email validator

#Usage

    $("input#email").validEmail() returns true if valid, false if invalid.

#Examples

This will bind the email validation check on the blur event. If it validates it will run the success handler. When it fails it will run the failure hanlder.

    $("input.email").validEmail({on:"blur", success:function(){
        $(this).removeClass("error").addClass("valid");
    }, failure:function(){
        $(this).removeClass("valid").addClass("error");
    }});
You can also pass in a true value to testInitially to test as the code gets executed aswell as when the event is triggered.
