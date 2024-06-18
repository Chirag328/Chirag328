<!DOCTYPE html>
<html>
<head>
<title>Registration Form</title>
<style>
  
   h2{
    background: linear-gradient(to right, #30cfd0, #330867 100%);
    -webkit-background-clip: text;
  }
  .card{
    background: linear-gradient(to right, #30cfd0, #330867 100%);
    -webkit-background-clip: text;
    color: transparent;
  }
  .card {
  box-shadow:  0 4px 8px 0 rgb(3, 250, 246); /* this adds the "card" effect */
  padding: 32px;
  background-size: cover;
  margin-top: 80px;
  box-sizing: content-box;
  object-fit: contain;
  height: auto;
  width: 300px;
  margin-left: 600px;
  border-radius: 20px;
  background-color:rgb(6, 21, 151);
  transition:5s;

}
.card-container :hover{
  box-shadow:0 3px 3px 0 rgb(6, 14, 17);
  ;

}
.card-container{
  padding: 4px 16px;

}

.button{
  color: blue;
}
.custom-select {
  position: relative;
  font-family: Arial;
}

.custom-select select {
  display: none; 
}

.select-selected {
  background-color: DodgerBlue;
}

.select-selected:after {
  position: absolute;
  content: "";
  top: 14px;
  right: 10px;
  width: 0;
  height: 0;
  border: 6px solid transparent;
  border-color: #fff transparent transparent transparent;
}

.select-selected.select-arrow-active:after {
  border-color: transparent transparent #fff transparent;
  top: 7px;
}

.select-items div,.select-selected {
  color: #ffffff;
  padding: 8px 16px;
  border: 1px solid transparent;
  border-color: transparent transparent rgba(0, 0, 0, 0.1) transparent;
  cursor: pointer;
}

.select-items {
  position: absolute;
  background-color: DodgerBlue;
  top: 100%;
  left: 0;
  right: 0;
  z-index: 99;
}

.select-hide {
  display: none;
}

.select-items div:hover, .same-as-selected {
  background-color: rgba(0, 0, 0, 0.1);
}

</style>
<script src="Register.js">
</script>
</head>
<body>
  <div class="card">
<form name="myForm" method="post">
  <h2>REGISTRATION FORM</h2>
  <div class="card-container">
Name<br><input type="text" placeholder="Your Name" name="fname"><br><br>
Address<br><textarea placeholder="Your Address"></textarea><br><br>
Contact No<br><input type="text" placeholder="Your Contact"><br><br>
Gender:<input type="radio" name="r1">
Male<input type="radio" name="r1">
Female<br><br>
Qualification <select>
                        <option>MSc</option>
                        <option>UG</option>
                        <option>HSc</option>
                   </select><br><br>
Hobbies:<input type="checkbox"> Singing<input type="checkbox"> Drawing <br><br><input type="checkbox">
Swimming<input type="checkbox"> Reading<br><br>
<button type="button" onclick="submit()">Submit</button>
<input type="reset" value="Reset">
<p id="demo"></p>
</table>
</div>
</form>
</div>
</body>
</html>
