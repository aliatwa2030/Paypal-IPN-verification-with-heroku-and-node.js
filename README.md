# heroku
heroku as lisenter for Instant Payment Notification (IPN) Simulator paypal Node JS

### In testConfig change app-name  with your herkuo app name
```
module.exports = {
	host: "https://(app-name).herokuapp.com"
}
```


### Use https://developer.paypal.com/developer/ipnSimulator to test payment 
in 'IPN handler URL' field put your heroku app url https://(app-name).herokuapp.com

### in web.js uncomment this for Simulating in localhost
```
//Object.setPrototypeOf(req.body, {});

/*
var port = 80;
app.listen(port);
var msg = 'Listening at http://localhost:' + port;
console.log(msg.green.bold);*/
```
