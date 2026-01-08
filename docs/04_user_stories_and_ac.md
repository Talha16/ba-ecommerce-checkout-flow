# User Stories & Acceptance Criteria – Checkout Flow

## Epic: Checkout Experience

---

### US-1: Proceed to Checkout
**As a** customer  
**I want** to start checkout from my cart  
**So that** I can purchase the items I selected.

**Acceptance Criteria**
- [ ] Given my cart has at least one item, when I select “Proceed to Checkout”, then I am taken to the checkout flow.
- [ ] Given my cart is empty, when I select “Proceed to Checkout”, then I see a message indicating the cart is empty and I cannot proceed.

---

### US-2: Choose Guest Checkout
**As a** customer  
**I want** to continue checkout as a guest  
**So that** I can complete my purchase without creating an account.

**Acceptance Criteria**
- [ ] When I begin checkout, I am offered “Sign In” or “Continue as Guest”.
- [ ] If I choose “Continue as Guest”, then I can continue to the shipping address step.
- [ ] Guest checkout does not require account creation to place an order.

---

### US-3: Enter Shipping Address
**As a** customer  
**I want** to enter my shipping address  
**So that** my order can be delivered correctly.

**Acceptance Criteria**
- [ ] Required fields include full name, address line 1, city, state, postal code, and country.
- [ ] If any required field is missing, then I see a clear error message and cannot proceed.
- [ ] If the postal code format is invalid for the selected country, then I see a validation message.

---

### US-4: Select Shipping Method
**As a** customer  
**I want** to see available shipping options  
**So that** I can choose based on cost and delivery speed.

**Acceptance Criteria**
- [ ] Given I have entered a valid shipping address, when I go to shipping method selection, then I can see available shipping options.
- [ ] Each shipping option displays price and estimated delivery date.
- [ ] If no shipping options are available, then I see an informative message and cannot proceed until resolved.

---

### US-5: Enter Payment Details
**As a** customer  
**I want** to enter payment information securely  
**So that** I can complete my purchase.

**Acceptance Criteria**
- [ ] Payment fields include card number, expiry date, CVV, and billing postal code.
- [ ] If I enter an invalid card number format, then I see a validation error.
- [ ] If payment authorization fails, then I see a retry message and remain on the payment step.

---

### US-6: Review Order Before Submission
**As a** customer  
**I want** to review my order details  
**So that** I can confirm they are correct before placing the order.

**Acceptance Criteria**
- [ ] The order review displays items, shipping address, shipping method, taxes, and total amount.
- [ ] I can return to edit shipping address, shipping method, or payment details before placing the order.

---

### US-7: Receive Order Confirmation
**As a** customer  
**I want** to receive confirmation after placing my order  
**So that** I know the purchase was successful.

**Acceptance Criteria**
- [ ] Given payment is successful, when I place the order, then an order ID is generated.
- [ ] The confirmation page displays the order ID and a success message.
- [ ] If the confirmation page fails to load, the order is still created and can be accessed via order history (conceptual).
