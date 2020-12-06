# background-color
<!DOCTYPE html>
<html>
    <head>
        <meta charset="uft-8">
        <title>background change</title>
    </head>
    <body>
        <button>change color</button>
        
        <script>
            const button = document.querySelector('button');

            let colors = ['red','black','pink','green','gray','blue'];

            function random(min,max){
              return Math.floor(Math.random() * (max-min) + min);  
            }

            function randomColor(array){
              let randomIdxNum = random(0,array.length);
              return array[randomIdxNum];
            }
            
            button.onclick = function(){
                document.body.style.backgroundColor = randomColor(colors);
  
            };
            

        </script>
    </body>
</html>
