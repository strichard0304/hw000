<!doctype html>
<html>
 <head>
  <meta charset="UTF-8">
   <title>D3 Course</title>
   <script src="https://d3js.org/d3.v3.js"></script>
   <style>
       p{
           border: 2px solid red;
           height: 30px;
           width: 80px;
           text-align: center;
           line-height: 30px;
       }
   </style>
 </head>
 <body>
   <p></p>
   <input type="button" onclick="launch()" value="啟動"/>
   <script>
       function random(N,M){
           return Math.ceil(Math.random()*(M-N)+N);
       }
       function launch(){           
           var rand=random(1911,2016);
           var body = d3.select("body>p");
           body.text(rand);
       }
       
       
   </script>  
  
 </body>
</html>