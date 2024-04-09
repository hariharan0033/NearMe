# Ex04 Places Around Me
## Date: 09/04/2024

## AIM
To develop a website to display details about the places around my house.

## DESIGN STEPS

### STEP 1
Create a Django admin interface.

### STEP 2
Download your city map from Google.

### STEP 3
Using ```<map>``` tag name the map.

### STEP 4
Create clickable regions in the image using ```<area>``` tag.

### STEP 5
Write HTML programs for all the regions identified.

### STEP 6
Execute the programs and publish them.

## CODE

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chennai Metro</title>
    <style>
        img,h1{
            display: inline;
        }
        h1{
            margin: none;
            position: absolute;
            top: 0%;
            right: 15%;
        }
        
    </style>
</head>
<body>
    
    <img src="map.png" width="1000px" alt="" usemap="#mapview" onmousemove="coordinate(event)" >
    <map name="mapview">
        <area shape="rect" coords="140,165,310,235" href="https://www.magicbricks.com/blog/koyambedu-metro-station/130572.html" title="koyambedu">
        <area shape="rect" coords="260,310,401,372" href="https://chennaimetrorail.org/vadapalani-metro-station-fare-table/" title="Vadapalani">
        <area shape="rect" coords="246,55,572,407" href="https://yometro.com/anna-nagar-east-metro-station-170032" title="Anna Nagar">
        <area shape="rect" coords="649,81,850,147" href="https://yometro.com/chennai-central-metro-station-170004" title="Chennai Central">
    </map>
    <h1>Chennai Metro</h1><br>
    x <input type="text" name="" id="x">
    y <input type="text" name="" id="y">



    <script>
        function coordinate(event){
            let x = event.clientX;
            let y = event.clientY;
            document.getElementById("x").value = x;
            document.getElementById("y").value = y;
        }
    </script>
</body>
</html>

```

## OUTPUT
![Screenshot (212)](https://github.com/hariharan0033/NearMe/assets/125666185/6b870f26-e5fa-4974-84f4-2d2806161a35)

![Screenshot (213)](https://github.com/hariharan0033/NearMe/assets/125666185/23478d93-7e82-4251-a4e4-dbee8dc4238e)







## RESULT
The program for implementing image maps using HTML is executed successfully.
