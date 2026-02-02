# BR-03: Delivery and billing address cannot be edited during checkout

### Summary
User cannot edit delivery or billing address details during the checkout process.

### Environment
- OS: MacOS 26.1
- Browser: Chrome (144.0.7559.97)
- Application: Automation Exercise
- URL: https://automationexercise.com

### Preconditions
- User is logged in
- User has an existing account with saved address details
- At least one product is added to the cart
- User is on the checkout page

### Steps to Reproduce
1. Review delivery and billing address details

### Expected Result
- User can edit delivery and billing address details during checkout  
  **or**
- User is provided with a clear option to update address information

### Actual Result
- Addresses fields are displayed as read-only
- No option to edit or update addresses information is available during checkout

### Severity
Medium

### Priority
Medium

### Notes
This behavior may be intentional; however, the lack of edit or navigation options may negatively impact user experience.  
In real-world e-commerce applications, users are typically allowed to update or select address details during checkout.
