# Cart Test Cases

### TC-01: User can add a product to the cart from main page

**Preconditions**
- User is on the main page

**Steps**
1. Select a product from the product list
2. Click the 'Add to Cart' button
3. Open the cart page from popup

**Expected Result**
- Selected product is added to the cart
- Product name, price, and quantity are displayed correctly

**Priority:** High  
**Type:** Functional, Smoke

---

### TC-02: User can add a product to the cart from product page

**Preconditions**
- User is on the product page

**Steps**
1. Click the 'Add to Cart' button
2. Open the cart page from popup

**Expected Result**
- Selected product is added to the cart
- Product name, price, and quantity are displayed correctly

**Priority:** High  
**Type:** Functional, Smoke

---

### TC-03: User can add multiple products to the cart

**Preconditions**
- User is on the main page

**Steps**
1. Add the first product to the cart
2. Add the second product to the cart
3. Open the cart page from popup

**Expected Result**
- Both products are displayed in the cart
- Each product has correct price and quantity

**Priority:** High  
**Type:** Functional

---

### TC-04: User can update product quantity in the cart

**Preconditions**
- Cart contains at least one product

**Steps**
1. Open the cart page
2. Increase product quantity

**Expected Result**
- Product quantity is updated
- Total price is recalculated correctly

**Priority:** High  
**Type:** Functional, Regression

---

### TC-05: User can remove a product from the cart

**Preconditions**
- Cart contains at least one product

**Steps**
1. Open the cart page
2. Remove a product from the cart

**Expected Result**
- Product is removed from the cart
- Cart is updated accordingly

**Priority:** High  
**Type:** Functional

---

### TC-06: Cart is empty after removing all products

**Preconditions**
- Cart contains multiple products

**Steps**
1. Open the cart page
2. Remove all products from the cart

**Expected Result**
- Cart is empty
- Empty cart message is displayed

**Priority:** Medium  
**Type:** Functional

---

### TC-07: Cart state is preserved after page refresh

**Preconditions**
- Cart contains at least one product

**Steps**
1. Open the cart page
2. Refresh the page

**Expected Result**
- Cart content remains unchanged after refresh

**Priority:** Medium  
**Type:** Functional, Regression

---

### TC-08: User can continue shopping after closing popup

**Preconditions**
- User is on the product page

**Steps**
1. Click the 'Add to Cart' button
2. Click 'Continue Shopping' button on popup

**Expected Result**
- Other 'Add to Cart' buttons are clickable

**Priority:** Medium  
**Type:** Functional, Regression

---

### Note:
In a real testing project, additional test cases would be added to cover price calculation edge cases,
stock limits, maximum quantity rules, and cart behavior for logged-in vs guest users.
