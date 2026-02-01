# Checkout Test Cases

### TC-01: User can proceed to checkout with products in cart

**Preconditions**
- Cart contains at least one product
- User is on the cart page

**Steps**
1. Click the 'Proceed To Checkout' button

**Expected Result**
- User is navigated to the checkout page
- Order and its summary are displayed correctly

**Priority:** High  
**Type:** Functional, Smoke

---

### TC-02: Guest user is prompted to login or register during checkout

**Preconditions**
- Cart contains at least one product
- User is not logged in
- User is on the cart page

**Steps**
1. Click the 'Proceed To Checkout' button

**Expected Result**
- User is prompted to login or registrate
- "Popup with links to login and registration page is displayed

**Priority:** High  
**Type:** Functional, Smoke

---

### TC-03: User is directed to card credential page with valid checkout data

**Preconditions**
- User is logged in
- Cart contains at least one product
- User is on the checkout page

**Steps**
1. Verify delivery address details
2. Enter a comment (optional)
3. Click the 'Place Order' button

**Expected Result**
- User is redirected to card credentials page

**Priority:** High  
**Type:** Functional, Smoke

---

### TC-04: Order total matches cart total during checkout

**Preconditions**
- Cart contains multiple products
- User is on the checkout page

**Steps**
1. Open the cart page and note the total price
2. Proceed to checkout
3. Verify the total price on checkout page

**Expected Result**
- Total price on checkout page matches cart total

**Priority:** High  
**Type:** Functional, Regression

---

### TC-05: User can complete payment with valid payment details

**Preconditions**
- User is on the payment page

**Test Data (example)**
- Name: Test Test
- Card number: 4111 1111 1111 1111
- Expiry date: 12/30
- CVV: 123

**Steps**
1. Enter valid payment details
2. Click the 'Pay and Confirm Order' button

**Expected Result**
- Payment is successful
- Order confirmation message is displayed
- Download invoice button is displayed

**Priority:** High  
**Type:** Functional, Smoke

---

### TC-5: Payment fails with invalid expiry date

**Preconditions**
- User is on the payment page

**Test Data (example)**
- Name: Test Test
- Card number: 4111 1111 1111 1111
- Expiry date: 01/20
- CVV: 123

**Steps**
1. Enter invalid payment details
2. Click the 'Pay and Confirm Order' button

**Expected Result**
- Payment is rejected
- Appropriate error message is displayed

**Priority:** High  
**Type:** Functional, Regression

---

### TC-6: Payment fails with invalid card number

**Preconditions**
- User is on the payment page

**Test Data (example)**
- Name: Test Test
- Card number: 4111 1111 1111 11
- Expiry date: 11/30
- CVV: 123

**Steps**
1. Enter invalid payment details
2. Click the 'Pay and Confirm Order' button

**Expected Result**
- Payment is rejected
- Appropriate error message is displayed

**Priority:** High  
**Type:** Functional, Regression

---

### TC-7: Payment fails with invalid CVV

**Preconditions**
- User is on the payment page

**Test Data (example)**
- Name: Test Test
- Card number: 4111 1111 1111 1111
- Expiry date: 11/30
- CVV: 000

**Steps**
1. Enter invalid payment details
2. Click the 'Pay and Confirm Order' button

**Expected Result**
- Payment is rejected
- Appropriate error message is displayed

**Priority:** High  
**Type:** Functional, Regression

---

### TC-8: Cart is cleared after successful order placement

**Preconditions**
- User has successfully completed payment

**Steps**
1. Navigate to the cart page

**Expected Result**
- Cart is empty
- Previously ordered products are not displayed

**Priority:** Medium  
**Type:** Functional

---

### TC-9: User can download invoice after successful order

**Preconditions**
- User has completed an order
- User is on the order confirmation page

**Steps**
1. Click the 'Download Invoice' button

**Expected Result**
- Invoice is downloaded successfully
- Invoice contains correct order details

**Priority:** Low  
**Type:** Functional

### Note:
In a real testing project, additional test cases would be added to cover
payment gateway timeouts, payment field validation, double-click protection, 
duplicate payments, and network interruptions during payment processing
