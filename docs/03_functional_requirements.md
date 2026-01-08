# Functional Requirements – Checkout Flow

## FR-1: Initiate Checkout
- The system shall allow a customer to initiate checkout from the cart page.
- The system shall prevent checkout if the cart is empty.

## FR-2: Guest and Registered Checkout
- The system shall allow customers to proceed as a guest or sign in.
- The system shall not require account creation to complete checkout.

## FR-3: Shipping Address Capture
- The system shall allow customers to enter a shipping address.
- The system shall validate required address fields before allowing the user to proceed.
- The system shall display clear error messages for missing or invalid address information.

## FR-4: Shipping Method Selection
- The system shall display available shipping methods based on the shipping address.
- The system shall show delivery estimates and costs for each method.
- The system shall allow the customer to select one shipping method.

## FR-5: Payment Information
- The system shall allow customers to enter payment details securely.
- The system shall validate payment information before submission.
- The system shall handle payment authorization failures and display a retry message.

## FR-6: Order Review
- The system shall display an order summary before order submission.
- The system shall allow customers to review items, shipping details, and total cost.

## FR-7: Order Confirmation
- The system shall generate an order confirmation upon successful payment.
- The system shall display an order confirmation message to the customer.

