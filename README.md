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
    // https.get() generates an http.IncomingMessage object aka res argument in the callback function executed when the response is received.
    https.get(url, function(response){
      console.log(response.statusCode);
    
    response.on('data', function(data){
      // console.log(data) -> Data in form of hexadecimal
      const weatherData = JSON.parse(data) 
      // JSON.parse -> parse a JSON string and convert it into JS object(dictionary)
      const temp = weatherData.main.temp
      const weatherDescription = weatherData.weather[0].description
    
    
    
