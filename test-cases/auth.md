# Authentication Test Cases

### TC-01: Account is not created if registration is not completed

**Preconditions**
- User is on the main page
- User is not registered

**Test Data (example)**
- name: test
- email: test_user_01@example.com

**Steps**
1. Click the 'Signup / Login' button
2. Enter valid name and email using test data in 'New User Signup!' form
3. Click the 'Signup' button
4. Go to Home page before submitting the registration form

**Expected Result**
- User account is not created 
- User is on the main page
- User is not logged in

**Priority:** High  
**Type:** Functional, Regression

---

### TC-02: User can register with valid data

**Preconditions**
- User is on the main page
- User is not registered

**Test Data (example)**
- name: test
- email: test_user_01@example.com
- password: test_test_test
- first name: test
- last name: test
- address: 12 Bridge Street
- country: Australia
- state: NSW
- city: Sydney
- zipcode: 2000
- mobile number: 0400000000

**Steps**
1. Click the 'Signup / Login' button
2. Enter valid name and email using test data in 'New User Signup!' form
3. Click the 'Signup' button
4. Fill in account information using test data
5. Submit the registration form

**Expected Result**
- User account is created successfully
- 'Account Created!' confirmation page is displayed
- User can continue using the 'Continue' button

**Priority:** High  
**Type:** Functional, Smoke

---

### TC-03: User can login with valid data

**Preconditions**
- User email already exists in the system
- User is on the main page
- User is not logged in

**Test Data (example)**
- email: test_user_01@example.com
- password: test_test_test

**Steps**
1. Click the 'Signup / Login' button
2. Enter valid email and password using test data in 'Login to your account' form
3. Click the 'Login' button

**Expected Result**
- User is logged in successfully
- User is redirected to the main page

**Priority:** High  
**Type:** Functional, Smoke

---

### TC-04: Registration fails with already registered email

**Preconditions**
- User email already exists in the system
- User is on the main page

**Test Data (example)**
- name: test
- email: test_user_01@example.com

**Steps**
1. Click the 'Signup / Login' button
2. Enter valid name and email using test data in 'New User Signup!' form
3. Click the 'Signup' button

**Expected Result**
- Registration is rejected
- Validation message 'Email Address already exist!' is displayed

**Priority:** High  
**Type:** Functional, Regression

---

### TC-05: Login fails with invalid credentials

**Preconditions**
- User has an existing account
- User is not logged in
- User is on the main page

**Test Data (example)**
- email: test_user_01@example.com
- password: 12345678

**Steps**
1. Click the 'Signup / Login' button
2. Enter incorrect email or password in 'Login to your account' form
3. Submit the login form

**Expected Result**
- Login is rejected
- Validation message 'Your email or password is incorrect!' is displayed

**Priority:** Medium  
**Type:** Functional

---

### TC-06: Registration fails with invalid email format

**Preconditions**
- User is on the main page
- User is not registered

**Test Data (example)**
- name: test
- email: test_user_01

**Steps**
1. Click the 'Signup / Login' button
2. Enter name and invalid email format in 'New User Signup!' form
3. Click the 'Signup' button

**Expected Result**
- Registration is rejected
- Validation message is displayed for invalid email format

**Priority:** Medium  
**Type:** Functional

---

### TC-07: Registration fails when name field is empty

**Preconditions**
- User is on the main page
- User is not registered

**Test Data (example)**
- email: test_user_01@test.com

**Steps**
1. Click the 'Signup / Login' button
2. Leave name field empty
3. Click the 'Signup' button

**Expected Result**
- Registration is rejected
- Required name field validation message is displayed

**Priority:** High  
**Type:** Functional, Regression

---

### TC-08: Registration fails when email field is empty

**Preconditions**
- User is on the main page
- User is not registered

**Test Data (example)**
- name: test
  
**Steps**
1. Click the 'Signup / Login' button
2. Leave email field empty
3. Click the 'Signup' button

**Expected Result**
- Registration is rejected
- Required email field validation message is displayed

**Priority:** High  
**Type:** Functional, Regression

---

### TC-09: Login fails with empty email

**Preconditions**
- User has an existing account
- User is not logged in
- User is on the main page

**Test Data (example)**
- password: test_test_test

**Steps**
1. Click the 'Signup / Login' button
2. Leave email field empty
3. Click the 'Login' button

**Expected Result**
- Login is rejected
- Required email field validation message is displayed

**Priority:** High  
**Type:** Functional

---

### TC-10: Login fails with empty password

**Preconditions**
- User has an existing account
- User is not logged in
- User is on the main page

**Test Data (example)**
- email: test_user_01@example.com
  
**Steps**
1. Click the 'Signup / Login' button
2. Leave password field empty
3. Click the 'Login' button

**Expected Result**
- Login is rejected
- Required password field validation message is displayed

**Priority:** High  
**Type:** Functional

---

### Notes

In a real production project, additional test cases would be created to validate each field of the registration form individually (e.g. first name, last name, address, postcode, phone number).

These checks are intentionally not listed here to avoid repetitive test cases. Field-level validations would typically be covered through exploratory testing and automated checks using varied test data.

