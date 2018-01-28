# Paypal IPN verification with heroku and node.js
heroku as lisenter for Instant Payment Notification (IPN) Simulator paypal Node JS

### herkuo change
In testConfig change app-name  with your herkuo app name
```
module.exports = {
	host: "https://(app-name).herokuapp.com"
}
```


### test fake payment
Use https://developer.paypal.com/developer/ipnSimulator to test payment 
in 'IPN handler URL' field put your heroku app url https://(app-name).herokuapp.com

### edit web js 
in web.js uncomment this for Simulating in localhost
```
//Object.setPrototypeOf(req.body, {});

/*
var port = 80;
app.listen(port);
var msg = 'Listening at http://localhost:' + port;
console.log(msg.green.bold);*/
```
### cmd git
initial git

```
git init
git add .
git commit -m 'message'
```

run fake test
```
npm test
node web.js
```
change herku running app

```
heroku git:remote -a appname
git push -f heroku master
```
### install mocha
```
$ npm install --save-dev mocha
```
Set up a test script in package.json:

```json
"scripts": {
    "test": "mocha"
  }
```

http://markmiyashita.com/blog/install_heroku_and_deploy_your_app/






