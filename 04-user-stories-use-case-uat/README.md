# 04 · Scheduled Food Delivery – User Stories, Use Case and UAT

## Scenario

A food-delivery company plans to let customers schedule orders for a later date and time. Customers select a delivery slot, confirm an address and receive confirmation; operations staff need to view scheduled orders.

## What was done

- Identified **7 actors** (Customer, Operations Staff, Restaurant, Rider, Payment Gateway, Maps service, Notification service)
- Wrote **5 user stories** with **Given / When / Then acceptance criteria**
- Wrote a **detailed use case** (UC-01 Schedule an order) with preconditions, 13-step main flow, 6 alternate/exception flows and postconditions
- Designed **8 UAT test cases** with ID, scenario, preconditions, steps, test data, expected result and Pass/Fail field
- Built **traceability** from user stories → acceptance criteria → test cases

## User stories

| ID | User story |
|----|------------|
| US-01 | As a customer, I want to choose a future delivery date and time slot, so that my food arrives when I need it. |
| US-02 | As a customer, I want to confirm and validate my delivery address, so that the order reaches the right place. |
| US-03 | As a customer, I want a confirmation and reminder, so that I know my order is booked. |
| US-04 | As a customer, I want to change or cancel before the cut-off, so that I can adjust when plans change. |
| US-05 | As operations staff, I want to view and filter scheduled orders, so that I can plan restaurant and rider capacity. |

## Edge cases covered in UAT

| Edge case | Test cases |
|-----------|------------|
| Unavailable / full slots, slot filling during checkout | UAT-02, UAT-03 |
| Invalid address and address outside the delivery zone | UAT-04, UAT-05 |
| Scheduling outside the allowed window (under 2 hours / beyond 7 days) | UAT-06 |

## Deliverables

- [User_Stories_Use_Case_Scheduled_Delivery.pdf](User_Stories_Use_Case_Scheduled_Delivery.pdf) — user stories, acceptance criteria, use case, UAT plan and traceability
- [UAT_Test_Cases_Scheduled_Delivery.xlsx](UAT_Test_Cases_Scheduled_Delivery.xlsx) — 8 test cases with Pass/Fail dropdown and auto-calculated execution summary
