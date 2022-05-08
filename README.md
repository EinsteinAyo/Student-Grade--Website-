# Student-Grade--Website-
Student Grade Website
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">

    <title>God is good</title>
  </head>
  <body>
  <style>
  body {
      background-color : darkcyan;
      padding:4%;
      color:whitesmoke;
  }
  .red{
      background-color:red;
      padding:4%;
  }
  .blue{
      background-color:blue;
      padding:4%;
  }
  .white{
      background-color:whitesmoke;
      color:black;
  }
  .green{
      background-color: orange;
      color:blue;
  }
  </style>
    <h1>Student Grade Calculator</h1>

<div class="container">
  <div class="row">
    <div class="col-4 red">Column</div>
    
      <h2>Your percentage is:</h2>
<h3 id="percentage"></h3>
<h2>Your grade is:</h2>
<h3 id="grade">A</h3>
    </div>
    <div class="col-8 blue">
      Column
    </div>
    
    <h1>Enter Your Marks</h1>
 
  <div class="mb-3">
    
    <input type="text" class="form-control" placeholder="Maths" id="Maths" >
    
  
  <div class="mb-3">
    
    <input type="text" class="form-control" placeholder="Physics" id="Physics">
   
  <div class="mb-3">
  
  <input type="text" class="form-control" placeholder="Chemistry" id="Chemistry"> 
  <div class="mb-3">
  
  <input type="text" class="form-control" placeholder="English" id="English"> </div>

  
  <button type="submit" onclick="getmark()" class="btn btn-primary">submit</button>
<div class="row"> 
<div class="col-12 white">
<h3 id="pass"> You have been passed</h3>
</div>
</div>


    
<!-- Footer -->
    <!-- Optional JavaScript; choose one of the two! -->

    <!-- Option 1: Bootstrap Bundle with Popper -->
    <footer>
    <div class="footer">
    <div class="col-12 green">
  <p id="footer">Builder: Isarinade Ayodeji<br>
  <a href="mailto: isarinadea@gmail.com.com">isarinadea@gmail.com</a></p> 
  </div>
  </div>
</footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" crossorigin="anonymous">
   
   function getmarks(){
       var Maths
=Number(document.getElementById("Maths").value);
       
    var English=Number(document.getElementById("English").value);  
  
   var Chemistry=Number(document.getElementById("Chemistry").value); 

 var Physics=Number(document.getElementById("Physics").value);
   
   var TotalMarks=400;
   var MarksObtained=Maths+English+Physics+Chemistry;
   
   var Percentage=(MarksObtained/TotalMarks)*100;
   
   document.getElementById("percentage).innerHTML=Percentage + "%";
      
       }
       var grade="";
       if (Percentage > 90){
           grade="A+";
       }
       else if(Percentage <90 && Percentage>80){
           grade="A";
       }
       else if(Percentage < 80 && Percentage > 75){
           grade="B+";
       }
       else if(Percentage < 60){
           grade="F";
       }
       document.getElementById("grade").innerHTML=grade;
       
       if (percentage<60){
           document.getElementById("pass").innerHTML="Sorry! You failed. Try next time"
       };
    </script>

  </body>
</html>
