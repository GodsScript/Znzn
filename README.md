<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Traffic Light</title>
  <style>
    body {
      text-align: center;
      font-size: 150px;
      color: white;
      font-family: Arial, Helvetica, sans-serif;
    }
  </style>
</head>
<body id="cloror">

<script>
  let lights = ["Green", "Yellow", "Red"];
  let time = [30000, 5000, 25000];
  let wholetime = 0;

  for (let i = 0; i <= lights.length; i++) {
    setTimeout(() => {
      if (lights[i] === "Green") {
        document.getElementById("cloror").style.backgroundColor = "green";
        
      } else if (lights[i] === "Yellow") {
        document.getElementById("cloror").style.backgroundColor = "yellow";
        
      } else {
        document.getElementById("cloror").style.backgroundColor = "red";
        
      }
    }, wholetime);
    wholetime += time[i];
  }
</script>

</body>
</html>
