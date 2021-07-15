# Ticket Engine Shopping Cart

The Ticket Engine Shopping Cart library renders a shopping cart or price list in a container element. If a eventId is supplied in the config object then the price list for the event will be rendered. Otherwise it will render the shopping cart content. 

The Ticket Engine Shopping Cart has 2 states:
1. Price list
2. Cart

The price list state renders a price list for an event. If the eventId option is supplied in the config object the price list state will be rendered. 

The cart state renders an overview of all tickets currently in the cart. This state will be rendered id no eventId option is supplied. 



## Usage

1. Include the following script in the ```<body>``` above any other JavaScript in your checkout page:  
```html
<script type="application/javascript" src="https://www.ticketengine.nl/resources/shopping-cart/v1/cart.js"></script>
```

2. Use the following CSS file:
```html
<link rel=stylesheet type=text/css href=https://www.ticketengine.nl/resources/shopping-cart/v1/cart.css>
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
    eventId: '<EVENT-UUID>',
    salesChannelId: '<SALES-CHANNEL-UUID>',
    registerId: '<REGISTER-UUID>'
});
</script>
```


## Configuration

Option  | Optional | Description | Default
:--- | :--- | :--- | :---
el | False | Css selector of the container element where cart or price list is rendered. | null
authUrl | True | Url of the Ticket Engine oAuth2 server. | https://auth.ticketengine.io
adminApiUrl | True | Admin API url. | https://admin-api.ticketengine.io
graphApiUrl | True | Graph API url. | https://graph-api.ticketengine.io
username | False | Shopping cart username. | null
eventId | True | If eventId is supplied price list will be rendered else render shopping cart. | null
salesChannelId | False |  | null 
registerId | False |  | null
customerId | True |  | null
defaultQuantity | True | Default pre filled quantity per price | 0
disablePaymentMethodSelection | True | Disable payment method selection | false
disableCartEditing | True | Disable the change cart content on checkout | false
language | True | Language settings object, see description below | null
onAddedToCart | True | Call back function that will be called when a ticket is added to the cart. | null 
onFinishedCartOperation | True | Call back function that will be called when a cart operation (add or remove ticket) is finished. Callback will be called with a order object. | ({order}) => {} 
onLoad | True | Call back function that will be called when a cart is loaded. Callback will be called with a order object. | ({order}) => {} 


### Language
Option  | Default
:--- | :---
type | Type
price | Price
quantity | Quantity
addToCart | Add to cart
change | Change
cancel | Cancel
cancelOrder | Cancel order
save | Save
totalPrice | Total
checkout | Checkout
reserve | Reserve
paymentMethod | Payment method
creditPayment | Payment
accountTokenLabel | Enter your account for payment of
accountTokenPlaceholder | Enter your account.
pay | Pay
free | Free
email | Email
emailPlaceholder | my.email@example.com
orderNotFound | Order not found.
orderTimeout | Order timeout.
orderCanceled | Order canceled.
orderCompleted | Order completed.
orderReserved | Order reserved.
noItems | Order is empty.
pendingItems | Order has unconfirmed tickets.
pendingItemsPleaseWait | Order has pending order line items. One moment please.
paymentProcessing | Processing payment.
noPrices | No prices found.
noCapacity | No capacity available for event.
loading | Loading...
tokenLabel | Enter your coupon code
tokenPlaceholder | Coupon code
tokenAddedLabel | Added coupons:
addToken | Add:
validatingToken | Validating coupon
accountTokenLabel | Enter your account for payment of
accountTokenPlaceholder | Enter your account.
selectTimeSlot | Select a time slot


