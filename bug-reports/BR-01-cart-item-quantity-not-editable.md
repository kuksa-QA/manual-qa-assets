# BR-01: Cart item quantity cannot be changed

### Summary
User is unable to change the quantity of products in the cart.

### Environment
- OS: MacOS 26.1
- Browser: Chrome (144.0.7559.97)
- Application: Automation Exercise
- URL: https://automationexercise.com

### Preconditions
- User is on the main page

### Steps to Reproduce
1. Add any product to the cart
2. Navigate to the cart page
3. Attempt to change the product quantity

### Expected Result
- User can increase or decrease the product quantity
- Cart total is updated accordingly

### Actual Result
- Product quantity cannot be edited
- Cart only allows removing items, not updating quantity

### Severity
Major

### Priority
High

### Notes
Lack of quantity control limits user ability to adjust order without removing and re-adding products.
