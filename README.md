<h1>Weather Dashboard with OpenWeather API and AWS S3 Bucket</h1>
<p>Day 1 Lab from the 30 Days of DevOps Challenge. This repository was cloned from https://github.com/ShaeInTheCloud/30days-weather-dashboard to replicate the following diagram.</p>
<p>To complete this challenge, I followed along ShaeInTheCloud's YouTube video. That video can be found here: https://www.youtube.com/watch?v=A95XBJFOqjw</p>
![image](https://github.com/user-attachments/assets/871d4dea-aed7-4e93-b30f-5619b42bf2bb)
<h2>Prerequisits</h2>
<p>To run this script, the following prerequisites are needed.</p>
<ul>
  <li>OpenWeather API Key</li>
  <li>AWS Access Key ID</li>
  <li>AWS Access Key ID</li>
</ul>
<h2>Weather_dashboard.py</h2>
<p>When the weather_dashboard.py file is first run, it checks to see if the AWS S3 bucket listed in the .env file already exists. If the S3 bucket does not exist, then the bucket is created using the create_bucket_if_not_exists method. </p>
<p>After verifying that an S3 bucket exists, the next step in the process is to fetch the weather data using the OpenWeather API. The fetch_weather method is used for each city that is listed in the cities list.  Weather data that is gathered for each city includes the city’s temperature, feels like, humidity and description.</p>
<p>Weather data for each city is then saved to an S3 bucket.</p>
![image](https://github.com/user-attachments/assets/27954271-cb99-4f80-be9c-ed439ebcb5c2)
