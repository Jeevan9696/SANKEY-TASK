# SANKEY-TASK1
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    
    <style>
        *{
            box-sizing: border-box;
            margin: 0;
            overflow: hidden;

        }
        
        .sec form{
            height: 100vh;
        }
        form{
            display: flex;
            flex-direction: column;
            align-items: center;
            font-family: 'Times New Roman', Times, serif;
            font-size:large;
            justify-content: flex-start;
        }
        section{
            display:grid;
            grid-template-columns: 1fr 1fr;
            justify-content: center;
            align-items: center;
            bottom: 0;
            margin-bottom: 0%;
            
        }
        p , h2, input , button{
            margin-top: 10px;
        }
        input[type='email'],input[type='password']{
            border-radius: 3px;
            width: 100%;
            height: 2.5em;
            background-color: rgb(225, 224, 221);
            padding: 10px;
            outline: none;
            border: none;
        }
        span a{
            margin-left: 13px;
        }
        span{
            font-size:medium;
        }
        button{
            display: block;
            width: 100%;
            height: 2.8em;
            border: none;
            border-radius: 3px;
            
            cursor: pointer;
        }
        #email_error,#pass_error{
            margin-top: 5px;
            color: #c62828;
            font-size: smaller;
            background: rgba(255, 0, 0,0, 1);
            text-align: center;
            padding: 5px,8px;
            display: none;
        }
        #login-button{
            background-color: #04c35c;
            color: white;
            font-weight: bold;
            margin-bottom: 4px;
        }
        #register-button{
            background-color: #2d3748;
            color: white;
            font-weight: bold;
            align-items: center;
            justify-content: center;
            display: flex;
        }
        .bottom{
            position: absolute;
            bottom: 0;
        }
      



        /* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {
    body{
        background-image: url('mountain.jpg');
        background-attachment: fixed;
        background-position: center;
        background-clip: border-box;

    }
    section{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-top: 50px;
        

    }
    #image{
        display: none;
    }
    .bottom{
        background-color: rgba(255, 255, 255, 0.619);
    }
}

/* Small devices (portrait tablets and large phones, 600px and up) */



        
    </style>
</head>
<body>
    <section>
        <div class="sec" id="image"><img src="mountain.jpg" alt="" width="700em" height="727em""></div>
        
            <form action="#">
               <div>
                <p>Welcome back</p>
                <h2>Login to your account</h2>
                <p class="ftxt">Email</p>
                <input type="email" name="email" id="mail" placeholder="john.snow@gmail.com">
                <div id ="email_error">please check your email !!</div>
                <p class="ftxt">Password</p>
                <input type="password" name="password" id="pass" placeholder="**********">
                <div id ="pass_error">please check your password !!</div>
                <div><span><input type="checkbox" name="checkbox" id="checkbx">Remember me</span><span><a href="#">Forgot Password?</a></span></div>
                <button class="button" id="login-button" onclick="validate()">Login now </button>
                <button id="register-button"><img src="ggl.png" alt="" width="20px" height="20px">Or sign-in with google</button>
                <div class="bottom">Don't have an account?&nbsp;<a href="#">Join free today</a></div>
               </div>
               
            </form>
            
            
    </section>
    <script>
        function validate()
        {
         var email=document.getElementById("mail").value
         var password=document.getElementById("pass").value

         var email_error
         if(email=="sankey901@solutions.com" && password=="mindset") 
         (
            //   <a href = "http://127.0.0.1:5500/welcome.html"> </a>

             window.open("./welcome.html",'_blank')
            
         ) 
         else if(email=="sankey901@solutions.com"&& password != "mindset" )
         (
          document.getElementById("pass_error").style.display="block"
        //   alert("cheak email and password")
         )
         else if(email !="sankey901@solutions.com"&& password == "mindset" )
         (
             document.getElementById("email_error").style.display="block"
         )
         else
         (
            document.getElementById("pass_error").style.display="block",
            document.getElementById("email_error").style.display="block"
         )
              
        }

    </script>
</body>
</html>
          
          
 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Welcome</title>
    <style>
        h1{
            color: azure;
            margin-left: 540px ;
        }
    </style>
    
</head>
<body background="./Welcome page.png">
    <h1>Welcome Sankey!!</h1>
</body>
</html>         
