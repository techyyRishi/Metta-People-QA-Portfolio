# Metta People – Program Listing QA Stability Review

## Project Overview

This document presents a QA stability review of the Program-Type Facilitator Listing flow in Metta People.

The review focuses on making the Program listing experience more predictable, testable, and customer-safe by identifying areas that require stronger validation, clearer business rules, and improved workflow consistency.

The assessment covers the complete flow from Provider Program creation and bundled session configuration to Customer selection, booking request, and Provider approval or decline.

## Scope of Review

### 1. End-to-End Program Listing Flow
- Provider creates a Program listing.
- Existing or new 1:1 Sessions and Workshops are added.
- Program windows and child session schedules are configured.
- Provider publishes the listing.
- Customer selects a Program window and applicable sessions.
- Customer submits a booking request.
- Provider approves or declines the request.

### 2. Requirement & Business Rule Review
Reviewed the captured requirements around:

- Program window selection
- Multiple Workshop date selection
- 1:1 date and time selection
- Provider-configured availability
- Cross-date bundled sessions
- Booking approval and decline
- Program pricing
- Cancellation and rescheduling rules

Confirmed requirements and open business decisions were kept separate in the review.

### 3. QA Stability & Risk Areas

The report identifies six major stability areas:

- **Schedule Consistency:** Maintain consistency between Program windows, Workshop dates, and 1:1 availability.
- **Customer Selection:** Make selected sessions and available booking options clear.
- **Capacity Enforcement:** Prevent booking beyond configured capacity.
- **Bundle Identity:** Help customers identify the intended bundled 1:1 session.
- **Lifecycle Dependencies:** Define the impact of editing, closing, or deleting child listings.
- **Validation Feedback:** Provide clear explanations when an action cannot proceed.

### 4. Provider-Side Recommendations
- Prevent ambiguous or duplicate bundled session configurations.
- Preserve the identity and type of bundled sessions.
- Improve Save and Continue state clarity.
- Revalidate schedules after relevant changes.

### 5. Customer-Side Recommendations
- Validate selected dates and times against provider configuration.
- Make Workshop and 1:1 selection rules clear.
- Prevent impossible booking combinations.
- Provide clear feedback when no valid booking option exists.

### 6. Capacity & Booking Controls
- Display remaining capacity clearly.
- Enforce configured maximum seats.
- Prevent booking when capacity is exhausted.
- Maintain consistency between displayed availability and actual booking behaviour.

### 7. Recommended Stabilisation Priorities

The report proposes a priority-based approach:

- **P0:** Capacity enforcement and schedule validation.
- **P1:** 1:1 session identity, validation feedback, and lifecycle dependencies.
- **P2:** Business rule documentation and requirement clarification.

## Stakeholder Review & Presentation

I prepared this QA stability review to communicate identified observations and recommendations to the relevant project stakeholders.

The document was shared with the Manager, Developer, and Designer for review and discussion.

The objective was to bring attention to potential edge cases, requirement ambiguities, and improvements that could help make the Program listing flow more stable and predictable.

## QA Deliverable

📄 **[View Program Listing QA Stability Review (PDF)](./Program-Listing-QA-Stability-Review.pdf)**

## Skills Demonstrated

- Requirement Analysis
- Business Rule Validation
- End-to-End Flow Analysis
- Risk Identification
- Edge Case Analysis
- QA Recommendations
- Stakeholder Communication
- Product Stability Review

## Document Note

This report distinguishes QA observations, recommendations, confirmed requirements, and open business decisions. Recommendations should be validated against the final agreed product requirements.


