# Test Strategy — Automation Exercise
https://automationexercise.com/

## 1. Project Overview
Automation Exercise is a demo e-commerce web application that allows users to browse products (including seacrh), register accounts, manage carts, complete purchases.
Features such as an order details or order history page are intentionally excluded because they are not present in the application.

This test strategy defines the approach for validating core functionality, usability, and reliability of the current application from a QA perspective.

---

## 2. Test Objectives
- Verify that critical user flows work as expected
- Identify functional and usability defects early
- Ensure stable behavior across core features
- Provide confidence in releases through repeatable tests

---

## 3. Scope of Testing

### In Scope
- User registration/ login
- Product browsing and search
- Cart management (add/delete)
- Checkout flow (excluding real payments)
- UI behavior and validations
- Public API endpoints (where applicable)

### Out of Scope
- Performance and load testing
- Security penetration testing
- Third-party payment provider behavior
- Mobile native applications

---

## 4. Test Types
- Functional testing
- Smoke testing
- Regression testing
- Exploratory testing
- UI automation testing
- API testing

---

## 5. Test Environment
- Browser: Chrome (144.0.7559.97)
- OS: macOS
- Environment: Public demo environment
- Automation tools: Playwright (UI & API)

---

## 6. Test Data
- Test user accounts created for testing purposes
- Sample product data from the application
- Mock or predefined API responses when applicable

---

## 7. Risks and Mitigation

| Risk | Mitigation |
|-----|-----------|
| Unstable demo data | Use isolated test accounts |
| UI changes breaking tests | Prefer stable selectors |
| Limited API documentation | Validate responses via exploration |

---

## 8. Entry Criteria
- Application is accessible
- Test environment is available
- Test data is prepared

---

## 9. Exit Criteria
- All critical test cases executed
- No open critical or blocker defects
- Test results documented

---

## 10. Deliverables
- Test cases
- Bug reports
- Automated test suites
- Test execution reports
