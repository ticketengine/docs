# Ticket Engine Shopping Cart

The Ticket Engine Shopping Cart library renders a shopping cart or price list in a container element. If a eventId is supplied in the config object then the price list for the event will be rendered. Otherwise it will render the shopping cart content. 

## Usage

1. Include the following script in the ```<body>``` above any other JavaScript in your checkout page:  
```html
<script type="application/javascript" src="http://www.ticketengine.nl/resources/shopping-cart/v1/cart.js"></script>
```

2. Use the following CSS file:
```html
<link rel=stylesheet type=text/css href=http://www.ticketengine.nl/resources/shopping-cart/v1/te-shopping-cart.css>
```

3. Add shopping cart container element. for example:
```html
<div id="cart"></div>
```

4. Render cart or price list in container element.  
```html
<script type="application/javascript">
TicketEngineShoppingCart({
    el: '#cart',
    username: '<CART-USERNAME>',
    eventId: '<EVENT_UUID>',
    salesChannelId: '<SALES-CHANNEL-UUID>',
    registerId: '<REGISTER-UUID>'
});
</script>
```


## Configuration

Option  | Optional | Description | Default
:--- | :--- | :--- | :---
el | False | Container element where cart or price list is rendered. | null
authUrl | True | Url of the Ticket Engine oAuth2 server. | https://auth.ticketengine.io
adminApiUrl | True | Admin API url. | https://admin-api.ticketengine.io
graphApiUrl | True | Graph API url. | https://graph-api.ticketengine.io
username | False | Shopping cart username. | null
eventId | True | If eventId is supplied price list will be rendered else render shopping cart. | null
salesChannelId | False |  | null 
registerId | False |  | null
customerId | True |  | null
language | True | Language settings object, see description below | null
onAddedToCart | True | Call back function that will be called when a ticket is added to the cart. | null 


### Language
Option  | Default
:--- | :---
type | Type
price | Price
quantity | Quantity
addToCart | Add to cart
change | Change
cancel | Cancel
save | Save
totalPrice | Total
checkout | Checkout
paymentMethod | Payment method
pay | Pay
email | pay |  
emailPlaceholder | Enter your email address
orderNotFound | Order not found.
orderTimeout | Order timeout.
orderCanceled | Order canceled.
orderCompleted | Order completed.
paymentProcessing | Payment is processing.
loading | Loading...
noPrices | No prices found for event.

