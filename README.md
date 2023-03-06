<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body {font-family: Arial, Helvetica, sans-serif;}

/* Full-width input fields */
input[type=text], input[type=password] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  box-sizing: border-box;
}

/* Set a style for all buttons */
button {
  background-color: #3e4fec;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  cursor: pointer;
  width: 100%;
}

button:hover {
  opacity: 0.8;
}

/* Extra styles for the cancel button */
.cancelbtn {
  width: auto;
  padding: 10px 18px;
  background-color: #f44336;
}

/* Center the image and position the close button */
.imgcontainer {
  text-align: center;
  margin: 24px 0 12px 0;
  position: relative;
}

.container {
  padding: 16px;
}

span.psw {
  float: right;
  padding-top: 16px;
}



/* Modal Content/Box */
.modal-content {
  background-color: #fefefe;
  margin: 5% auto 15% auto; /* 5% from the top, 15% from the bottom and centered */
  border: 1px solid #888;
  width: 40%; /* Could be more or less, depending on screen size */
}

/* The Close Button (x) */
.close {
  position: absolute;
  right: 25px;
  top: 0;
  color: #000;
  font-size: 35px;
  font-weight: bold;
}

.close:hover,
.close:focus {
  color: red;
  cursor: pointer;
}

/* Add Zoom Animation */
.animate {
  -webkit-animation: animatezoom 0.6s;
  animation: animatezoom 0.6s
}

@-webkit-keyframes animatezoom {
  from {-webkit-transform: scale(0)} 
  to {-webkit-transform: scale(1)}
}
  
@keyframes animatezoom {
  from {transform: scale(0)} 
  to {transform: scale(1)}
}

/* Change styles for span and cancel button on extra small screens */
@media screen and (max-width: 300px) {
  span.psw {
     display: block;
     float: none;
  }
  .cancelbtn {
     width: 100%;
  }
}
</style>
</head>
<body>


@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap');
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}
body{
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    background-image: linear-gradient(
        45deg,#efefef 25%,rgba(46, 80, 160, 0.335) 25%,rgba(239,239,239,0) 75%,#efefef 75%,#efefef),linear-gradient(
        45deg,#1c4c8a 25%,rgba(239,239,239,0) 25%,rgba(239,239,239,0) 75%,#efefef 75%,#efefef);
}
.wrapper{
    width: 370px;
    padding: 30px;
    border-radius: 7px;
    background-color: #fff;
}
.wrapper header{
    font-size: 28px;
    font-weight: 500;
    text-align: center;
}
.wrapper form{
    margin: 40px 0 20px 0;
}
form :where(input, select ,button){
    width: 100%;
    outline: none;
    border: none;
    border-radius: 5px;
}
form p{
    font-size: 18px;
    margin-bottom: 5px;
}
form input{
    height: 50px;
    font-size: 17px;
    padding: 0 15px;
    border: 1px solid #999;
}
form input:focus{
    padding: 0 14px;
    border: 2px solid rgba(169, 183, 245, 0.972);
}
form .drop-list{
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 20px;
}
.drop-list .select-box{
    display: flex;
    height: 45px;
    width: 115px;
    border-radius: 5px;
    align-items: center;
    justify-content: center;
    border: 1px solid #999;
}
.select-box select ::-webkit-scrollbar{
    width: 80px;
}
.select-box select ::-webkit-scrollbar-track{
    background: #fff;
}
.select-box select ::-webkit-scrollbar-thumb{
    background: #8888;
    border-radius: 50%;
    border-right: 2px solid #fff;       
}
.select-box select{
    width: auto;
    font-size: 16px;
    margin: 0 -5px 0 5px;
}
.select-box img{
    max-width: 30px;
}
.drop-list .icon{
    cursor: pointer;
    font-size: 20px;
    margin-top: 30px;
    margin-left: 20px;
    margin-right: 20px;
}
form .exchange-rate{
    font-size: 17px;
    margin: 20px 0 30px 0;
}
form button{
    height: 52px;
    color: #fff;
    font-size: 17px;
    cursor: pointer;                    
    background: rgba(46, 80, 160, 0.685);
}
  

<div id="id01" class="modal">
  
  <form class="modal-content animate" action="/index.html" method="post">
    

    <div class="container">
      <label for="uname"><b>Username</b></label>
      <input type="text" placeholder="Enter Username" name="uname" required>

      <label for="psw"><b>Password</b></label>
      <input type="password" placeholder="Enter Password" name="psw" required>
        
      
      <button onclick="window.open('index.html');" target="_blank"> Login </button>
      <label>
        <input type="checkbox" checked="checked" name="remember"> Remember me
      </label>
    </div>

    <div class="container" style="background-color:#f1f1f1">
      <button type="button" onclick="document.getElementById('id01').style.display='none'" class="cancelbtn">Cancel</button>
      <span class="psw"><a href="#">Forgot Password?</a></span>
    </div>
  </form>
</div>

<script>
// Get the modal
var modal = document.getElementById('id01');

// When the user clicks anywhere outside of the modal, close it
window.onclick = function(event) {
    if (event.target == modal) {
        modal.style.display = "none";
    }
}
</script>

</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <title>CURRENCY COMPARISON</title>
</head>
<body>
    <div class="wrapper">
        <header>CURRENCY COMPARISON</header>
        <form action="#">
            <div class="amount">
                <p>Enter the Amount</p>
                <input type="text" value="1">
            </div>
            <div class="drop-list">
                <div class="from">
                    <p>From:</p>
                    <div class="select-box">
                       <img src="https://flagcdn.com/h20/us.png" alt="flag">
                       <select></select>
                    </div>
                </div>
                <div class="icon"><i class ="fas fa-exchange-alt"></i></div>
                <div class="to">
                    <p>To:</p>
                    <div class="select-box">
                       <img src="https://flagcdn.com/h20/np.png" alt="flag">
                       <select></select>
                    </div>
                </div>
            </div>
            <div class="exchange-rate">Getting Exchange Rate...</div>
            <button>Get Exchange Rate</button>
        </form>

    </div>    

    <script src = "Script.js"></script>
</body> 
</html>
