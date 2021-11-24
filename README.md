<!DOCTYPE html>  
<html>  
<head>  
<meta name="viewport" content="width=device-width, initial-scale=1">  
<style>  
body{  
  font-family: Calibri, Helvetica, sans-serif;  
  background-color: orange;  
}  
.container { 
  text-align:center; 
  padding: 20px;  
  background-color: white;  
}  
  
input[type=text], input[type=password], textarea {
  text-align:center;
  width: 80%;  
  padding: 10px;  
  margin: 10px 0 20px 0;  
  display: inline-block;  
  border: 0;  
  box-shadow:0 0 15px 4px rgb(30, 30, 185);
  border-radius:10px;
  background: #f1f1f1;  
}  
input[type=text]:focus, input[type=password]:focus {  
  background-color: rgb(255, 211, 130);  
  outline: none;  
}




div {  
  padding: 10px 0;  
}  

.registerbtn { 
  border-radius:10px; 
  background-color: darkorange;  
  color: black;  
  padding: 16px 20px;  
  margin: 8px 0;  
  border: none;  
  cursor: pointer;  
  width: 50%;  
  opacity: 1;  
}  
.registerbtn:hover {  
  opacity: 0.5;  
}  
</style>
</head>



<body>  
<form action"form-handler.php" method="get">  
<div class="container">  
<center>  <h1> Registration Form</h1> </center>


<label> <b>First Name</b> </label><br>   
<input type="text" name="firstname" placeholder= "firstname" size="15" required />
<br>
<label> <b>Last Name</b> </label><br>   
<input type="text" name="lastname" placeholder="lastname" size="15"required />
<br>

<div>  
<label> <b>Gender</b></label><br>  
<input type="radio" value="Male" name="gender" checked > Male   
<input type="radio" value="Female" name="gender"> Female   
<input type="radio" value="Other" name="gender"> Other 
<br> 
</div>


<label> <b>Phone</b> </label><br> 
<input type="number" name="phone" placeholder="phone"  value="+372" size="12" required>   
<br>


<label for="Group"><b>Choose a Group:<b></label>
<select name="Group" id="Group">
  <option value="IVSB11">IVSB11</option>
  <option value="IVSB12">IVSB12</option>
  <option value="Teacher">Teacher</option>
</select><br><br>


<label for="email"><b>Email</b></label><br>
<input type="email" placeholder="Enter Email" name="email" required>  
<br>
<label for="psw"><b>Password</b></label><br> 
<input type="password" placeholder="Enter Password" name="psw" required>  
<br>  
<center><button type="submit" class="registerbtn">Send</button> </center>
</form>  
</body>  
</html>  
