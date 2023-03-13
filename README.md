# Learning_API

API (Application Programming Interface) which provides a list of available functions, data types and protocols for users to interact with the program

- Endpoint
- Path
- Parameter
- Authentication

Postman - free tool to test API

    const https = require('https');
    app.get('/', function(req, res){
    const url = ''
    
    https.get(url, function(response){
      console.log(response.statusCode);
    
    response.on('data', function(data){
      const weatherData = JSON.parse(data)
      const temp = weatherData.main.temp
      const weatherDescription = weatherData.weather[0].description
    
    
    
