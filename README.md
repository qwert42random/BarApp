# BarApp
App for customer loyalty

## Features
- Two apps: customer and bartender
- Also a server
- Customer has ID (can be in form QR code)
- Customer gets 1 point for every drink purchased
- Bartender gives customer points using their ID on the app
- App keeps track of customer points
- Customer can redeem points which removes drinks purchased from database
- Bartender has database of all customers and their points
- Transaction history stored somewhere

## API functions
- Login: username, password {"username" : "example", "password", "hash"} -> POST?
- Logout: shut down session
- Generate key
- Account creation {"RequestType" : int, "username" : "example", "email" : "example@example.com",  "password", "hash"} API -> Database 
- Account removal
- Redeeming points (subtracting) {}
- Adding points

200 Ok {"Response" : "Message", "Success" : bool} <- Server (Database)
401 Unauth (Key has been rejected) <- Server
