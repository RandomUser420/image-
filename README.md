# image-
make screenshots of video

<html>
  <head>
    <script src="p5.min.js"></script>
    <script src="p5.gui.js"></script>
    <script src="quicksettings.js"></script>
    <script src="p5.dom.js"></script>
    <style>

    </style>
  </head>
  <body>
    <script>
   var button;
   var video;
   
   function setup(){
     createCanvas(390,240);
     video = createCapture(VIDEO);
     video.size(320,240);
     button = createButton('CLICK');
     button.mousePressed(snapshot);
     //capture.hide();
   }
    function snapshot(){
      image(video, 0, 0, 320, 240);
      
   }
     
    </script>
  </body>
</html>
