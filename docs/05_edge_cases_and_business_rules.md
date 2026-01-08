# Edge Cases & Business Rules – Checkout Flow

## Edge Cases

1. Customer closes the browser after submitting payment but before the confirmation page loads.
2. Address entered is valid but returns no shipping options.
3. Payment authorization times out due to network issues.
4. Customer attempts to refresh the page during payment submission.
5. Cart contents change (item out of stock) during checkout.
6. Session expires due to inactivity before order placement.

These scenarios require clear system handling to prevent duplicate orders, user confusion, or data inconsistency.

---

## Business Rules

- BR-1: Checkout cannot proceed with an empty cart.
- BR-2: All required shipping address fields must be completed before proceeding.
- BR-3: Only supported countries are eligible for shipping.
- BR-4: Payment must be authorized before an order confirmation number is generated.
- BR-5: Taxes and shipping costs are calculated based on the shipping address.
- BR-6: Orders with repeated payment failures may be flagged for review (conceptual).

---

## Light Automation / Intelligence Considerations (Conceptual)

- Address validation and formatting suggestions to reduce manual entry errors.
- Detection of repeated payment failures to prevent accidental duplicate charges.
- Logging of checkout drop-off points for future analysis and optimization.

These considerations are intended to improve reliability and user experience without adding unnecessary complexity.
