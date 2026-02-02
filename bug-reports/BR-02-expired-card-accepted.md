# BR-02: Payment form allows expired card details

### Summary
Payment form accepts expired card details without validation.

### Environment
- OS: MacOS 26.2
- Browser: Chrome (144.0.7559.110)
- Application: Automation Exercise
- URL: https://automationexercise.com

### Preconditions
- User is logged in
- At least one product is added to the cart
- User is on the payment page

### Steps to Reproduce
1. Enter valid card number and CVV (e.g. 4111 1111 1111 1111 and 123)
4. Enter an expired card expiry date (e.g. 01/20)
5. Click the 'Pay and Confirm Order' button

### Expected Result
- Expired card details are rejected
- User is informed that the card expiry date is invalid

### Actual Result
- Expired card details are accepted
- Order is processed successfully

### Severity
Major

### Priority
High

### Notes
Lack of expiry date validation may allow invalid payment data to be submitted.  
In real production systems, this validation is usually enforced client-side or by the payment gateway.
