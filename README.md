# Ex04 Places Around Me
# Date:11/04/2025
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE
map.html

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Places Around Chennai</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f3f3f3;
      text-align: center;
    }
    .container {
      width: 80%;
      margin: auto;
    }
    img {
      max-width: 100%;
      height: auto;
    }
    .details {
      margin-top: 20px;
    }
    .place-info {
      display: none;
      padding: 15px;
      background: #fff;
      margin: 10px auto;
      max-width: 600px;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
  </style>
  <script>
    function showInfo(id) {
      const allInfos = document.querySelectorAll('.place-info');
      allInfos.forEach(info => info.style.display = 'none');
      document.getElementById(id).style.display = 'block';
    }
  </script>
</head>
<body>
  <div class="container">
    <h1>Places in Chennai</h1>
    <h2>HARI KRISHNAN S (24006166)</h2>
    <img src="/static/map.png" usemap="#placesmap" alt="Map of places">
    <map name="map.png">
        <area target="" alt="koyembedu" title="koyembedu" href="koyembedu.html" coords="506,574,324,471" shape="rect">
        <area target="" alt="egmore" title="egmore" href="egmore.html" coords="1039,481,45" shape="circle">
        <area target="" alt="annanagar" title="annanagar" href="annanagar.html" coords="484,317,641,401" shape="rect">
        <area target="" alt="senmozhi poonga" title="senmozhi poonga" href="park.html" coords="910,685,44" shape="circle">
        <area target="" alt="vadapalani murugan temple" title="vadapalani murugan temple" href="temple.html" coords="551,636,643,730" shape="rect">
    </map>
</body>
</html>
```
koyembedu.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Koyembedu</title>
  <style>
    body { background-color: #cceeff; font-family: Arial; text-align: center; padding: 2em; }
    .card {
      background: #ffffff;
      padding: 2em;
      border-radius: 10px;
      max-width: 700px;
      margin: auto;
      box-shadow: 0 4px 12px rgba(0,0,0,0.15);
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>Koyembedu</h1>
    <p>Koyembedu is a major commercial and transport hub in Chennai. It is home to the <strong>Chennai Mofussil Bus Terminus (CMBT)</strong>, one of Asia’s largest bus terminals.</p>
    <p>The area also hosts the famous <strong>Koyembedu Market</strong>, known for fresh produce, flowers, and spices. You’ll see a blend of vibrant trade activity and bustling crowds from early morning.</p>
    <h3>Highlights:</h3>
    <ul style="text-align: left;">
      <li>CMBT – connects Chennai to all major cities in Tamil Nadu</li>
      <li>Koyembedu Wholesale Market Complex</li>
      <li>Local street food and budget shopping options</li>
    </ul>
    <p><em>Best time to visit: Early morning or late evening</em></p>
  </div>
</body>
</html>

```

egmore.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Egmore</title>
  <style>
    body { background-color: #ffe0b3; font-family: Arial; text-align: center; padding: 2em; }
    .card {
      background: #fff;
      padding: 2em;
      border-radius: 10px;
      max-width: 700px;
      margin: auto;
      box-shadow: 0 4px 12px rgba(0,0,0,0.15);
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>Egmore</h1>
    <p>Egmore is a cultural and historical hotspot in Chennai. It houses the renowned <strong>Government Museum</strong>, which showcases South Indian art, bronze statues, and ancient artifacts.</p>
    <p>The <strong>Egmore Railway Station</strong> is another iconic structure, serving thousands of commuters daily. Colonial-era buildings and leafy avenues give Egmore a classic charm.</p>
    <h3>Don’t Miss:</h3>
    <ul style="text-align: left;">
      <li>Government Museum and Connemara Library</li>
      <li>St. Andrew’s Church (The Kirk)</li>
      <li>Famous restaurants like Buhari and Hotel Saravana Bhavan</li>
    </ul>
    <p><em>Good for: History buffs, museum lovers, train travelers</em></p>
  </div>
</body>
</html>

```

annanagar.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Anna Nagar</title>
  <style>
    body { background-color: #d5f5d5; font-family: Arial; text-align: center; padding: 2em; }
    .card {
      background: #ffffff;
      padding: 2em;
      border-radius: 10px;
      max-width: 700px;
      margin: auto;
      box-shadow: 0 4px 12px rgba(0,0,0,0.15);
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>Anna Nagar</h1>
    <p>Anna Nagar is one of the most well-planned residential areas in Chennai, famous for its grid layout and peaceful atmosphere. It’s named after former Chief Minister C.N. Annadurai.</p>
    <p>You’ll find everything here—shopping malls, lush parks, schools, and hospitals. The area is also known for the <strong>Anna Nagar Tower Park</strong>, which features a 135-ft tower offering panoramic views.</p>
    <h3>Places to Explore:</h3>
    <ul style="text-align: left;">
      <li>Anna Nagar Tower Park</li>
      <li>VR Mall (nearby)</li>
      <li>Trendy cafes and ice cream parlors</li>
    </ul>
    <p><em>Perfect for: Families, evening walks, urban lifestyle</em></p>
  </div>
</body>
</html>

```

temple.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Vadapalani Murugan Temple</title>
  <style>
    body { background-color: #ffe6f0; font-family: Arial; text-align: center; padding: 2em; }
    .card {
      background: #ffffff;
      padding: 2em;
      border-radius: 10px;
      max-width: 700px;
      margin: auto;
      box-shadow: 0 4px 12px rgba(0,0,0,0.15);
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>Vadapalani Murugan Temple</h1>
    <p>This popular Hindu temple is dedicated to Lord Murugan. Known for its striking gopuram and vibrant rituals, it draws thousands of devotees daily.</p>
    <p>The temple also conducts <strong>marriage ceremonies</strong> regularly, and is considered very auspicious. Inside, the main deity’s idol is believed to have been installed by a devotee guided by a vision.</p>
    <h3>Temple Highlights:</h3>
    <ul style="text-align: left;">
      <li>Colorful gopuram with Murugan's life scenes</li>
      <li>Frequent religious ceremonies and processions</li>
      <li>Shops and prasadam counters nearby</li>
    </ul>
    <p><em>Spiritual vibe + beautiful architecture = must-visit</em></p>
  </div>
</body>
</html>

```

park.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Senmozhi Poonga</title>
  <style>
    body { background-color: #fffacd; font-family: Arial; text-align: center; padding: 2em; }
    .card {
      background: #ffffff;
      padding: 2em;
      border-radius: 10px;
      max-width: 700px;
      margin: auto;
      box-shadow: 0 4px 12px rgba(0,0,0,0.15);
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>Semmozhi Poonga</h1>
    <p>This beautiful botanical garden near Cathedral Road is a green oasis in the heart of the city. Managed by the Horticulture Department, it is home to over 500 species of plants and flowers.</p>
    <p>You’ll find themed gardens like herbal sections, bonsai collections, and water fountains, making it a photographer's and nature lover’s paradise.</p>
    <h3>Features:</h3>
    <ul style="text-align: left;">
      <li>Medicinal plant garden</li>
      <li>Children’s play area</li>
      <li>Walking paths, orchidarium, and rock gardens</li>
    </ul>
    <p><em>Recommended for: Families, tourists, nature photographers</em></p>
  </div>
</body>
</html>

```

# OUTPUT

![alt text](<Screenshot 2025-04-23 003228.png>)

![alt text](<Screenshot 2025-04-23 003248.png>)

![alt text](<Screenshot 2025-04-23 003312.png>)

![alt text](<Screenshot 2025-04-23 003347.png>)

![alt text](<Screenshot 2025-04-23 003407.png>)

![alt text](<Screenshot 2025-04-23 003435.png>)

# RESULT
The program for implementing image maps using HTML is executed successfully.
