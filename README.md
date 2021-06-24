# fizzfuzzgame
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fizz Buzz Game</title>
    <style>
        
* {
   font-family: myFirstFont;
}
        * {
            margin:0;
            padding:0;
            box-sizing:border-box;
        }
        .parent {
            width:100vw; 
            height:100vh;
            background-image:url("yellow.jpg")
         
        }

        .child {
            width:60vw;
            height:60vh;
          
            
  border-radius: 25px;
            position: absolute;
            left:50%;
            top:50%;
            transform:translate(-50%,-50%)
        }

   
        .child .head{
            color:#DC143C;
            font-family: sapi_windows_cp_get;
            padding-top: 30px;
            padding-left: 30px;
            margin:20px;
            font-size:60px;
           
            text-align: justify;
           
        }

        input[type=number] {
            
           width: 50%;
  padding: 12px 20px;
  margin: 8px 30px;
  box-sizing: border-box;
  border: none;
  border-radius: 25px;

             border-bottom: 2px solid red;
}

.sel{
        
    width: 50%;
  padding: 12px 20px;
  margin: 8px 30px;
  box-sizing: border-box;
  border: none;
  border-radius: 25px;

             border-bottom: 2px solid red;

}

.submit {
        
    width: 20%;
  padding: 2px 10px;
  margin: 4px 100px;
  box-sizing: border-box;
  background:#DC143C;
  color:black;
  font-size:30px;
  border-radius: 20px;

  border: none;
  cursor: pointer;

        
}

.para {
    color:#DC143C;
   
    font-size:40px;
    width: 100%;
  padding: 10px 10px;
  margin: 8px 30px;
}
  
        </style>
</head>
<body>
<div class="parent">

    <div class="child">
        <h1 class='head'>
            Fizz Buzz Game 

        </h1>
        <div class="sub-child"> 

        <form action="" method="POST">
            <input type="number" name="numone" placeholder="ENTER NUMBER">
       <!--     <input type="number" name="numtwo"  placeholder="ENTER NUMBER" > -->

       <!-- 
       
        <div>
            <select name="operation" class='sel'>
                <option value="add">Add</option>
                <option value="sub">Sub</option>
                <option value="mult">Multi</option>
                <option value="div">Div</option>

            </select>
            -->


      
        <div>
        <input type="submit" name="submit" value="submit" class="submit">
        </div>

        </form>
        </div>
          <div class="app">
        <p class="para">
            <?php
            if(isset($_POST['submit'])) {
                $num1=$_POST['numone'];
             #   $num2=$_POST['numtwo'];
              #  $Operation=$_POST['operation'];
               
                    if(($num1%3==0) && ($num1%5==0)){
                        echo "Fizz Buzz";
                      
                    }
                        
                    elseif($num1%3==0) {
                        echo "Fizz";
                        echo "</br>";
                     }
                        
                    elseif($num1%5==0) {
                        echo "Buzz";

                        echo "</br>";
                    }
                        
                    else {
                       echo "Not a multiple of 3 and 5 ";
                     echo "</br>";
                     }

                


            }
            

            ?>
        </p> 


        </div>


    
      
    
</div>

</div>


</body>
</html>
