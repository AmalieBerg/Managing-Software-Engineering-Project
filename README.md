# Meeting Lily's Requirements

A requirements engineering project for a local florist, "Lily's Florist". I interview the client, turn the interview into user stories, map one customer journey, write a traceable requirements specification, and design two Figma wireframes that show how the requirements become screens.

Built for the **Managing Software Engineering** course, Quantic School of Business and Technology (MSSE), September 2025. Solo project.

## Overview

Lily runs a florist business that handles walk-in sales, everyday gift orders, standing weekly orders and wedding and event work. Her pain points are manual inventory tracking, stock-outs and website strain during peak seasons, delivery scheduling that bunches drivers up, phone-based payments, and event projects scattered across notes and emails.

The project follows one chain from conversation to design:

Client interview → User stories → User journey map → Requirements specification → Wireframes

Every requirement points back to the user stories it serves, and every wireframe annotation points back to a requirement.

## What is in the project

| Deliverable | Summary |
|---|---|
| Requirements interview | A conversation with Lily the florist, used as the source for everything below |
| User stories | 23 stories following the INVEST criteria, across six personas plus mobile and desktop needs |
| User journey map | Event client journey for the persona "Wedding Sarah", in four phases |
| Requirements specification | 39 requirements (REQ-001 to REQ-039) in 11 categories, with a traceability matrix |
| Mockup wireframes | Landing page and consultation booking page, designed in Figma |

## User stories

The stories follow INVEST (Independent, Negotiable, Valuable, Estimable, Small, Testable). Each one addresses a specific pain point Lily described.

| Persona | Stories |
|---|---|
| Everyday gift buyer | 1 to 4 |
| Event client | 5 to 8 |
| Walk-in or immediate need | 9 to 10 |
| Regular customer with standing orders | 11 |
| First-time customer | 12 to 13 |
| Lily (the business owner) | 14 to 20 |
| Mobile and desktop users | 21 to 23 |

## User journey map

The journey covers the event client (stories 5 to 8). The workflow from the interview is: initial inquiry, consultation, design sketches, proposal and contract, timeline coordination, event delivery. I grouped it into four phases:

| Phase | Focus |
|---|---|
| Discover | Researching florists, comparing portfolios and pricing, making first contact |
| Consult | Booking a consultation, sharing vision and budget, reviewing the portfolio |
| Decide | Reviewing the proposal, comparing designs, negotiating, signing the contract |
| Execute | Tracking milestones, confirming final details, delivery and setup on the day |

For each phase the map shows user actions, goals and experiences, feelings and thoughts, pain points and opportunities, for the persona Wedding Sarah (28, marketing manager, planning her wedding with a budget of $3,000).

![User journey map](docs/user-journey-map.png)

## Requirements specification

39 requirements, split into functional (REQ-001 to REQ-026) and non-functional (REQ-027 to REQ-039). Each lists the user stories it traces to.

| Category | Requirements | Business pain point addressed |
|---|---|---|
| Customer experience and product display | REQ-001 to 005 | Customer confusion, lack of information |
| Inventory management | REQ-006 to 008 | Manual tracking, stock-outs during peaks |
| Payment processing | REQ-009 to 012 | Phone payment delays and errors |
| Delivery management | REQ-013 to 017 | Scheduling bunching, route inefficiency |
| Event management | REQ-018 to 022 | Manual project management, scattered information |
| Standing order management | REQ-023 to 025 | Informal order management |
| Personalization | REQ-026 | Gift customization needs |
| Performance and scalability | REQ-027 to 030 | Peak season system failures |
| Security and data protection | REQ-031 to 034 | Data protection and account security |
| Mobile and accessibility | REQ-035 to 037 | Cross-device functionality |
| Integration and backup | REQ-038 to 039 | System integration and data protection |

Examples of measurable requirements:

- Handle peak loads of 300 orders per day, three times normal capacity (REQ-027)
- Customer-facing pages respond in under 3 seconds (REQ-029)
- No more than 8 orders per 2-hour delivery slot (REQ-014)
- WCAG 2.1 Level AA accessibility (REQ-037)
- AES-256 encryption in transit and at rest (REQ-032)

## Wireframes

Two Figma wireframes connect the journey to the requirements. Yellow annotations on each wireframe name the requirement and the UX reasoning behind the design choice.

**Landing page** (REQ-001, 002, 005, 035, 036, 037). Product gallery with occasion, price and availability filters, availability badges for real-time inventory, two calls to action (Shop Now and Book Consultation) for different personas, and 44px touch targets for mobile.

![Landing page wireframe](docs/wireframe-landing-page.png)

**Consultation booking page** (REQ-018, 020, 037). Calendar with three months of advance availability, time slots shown only for the selected date, a 24-hour minimum lead time, an expectations panel that sets the proposal timeline at five days, and form validation that prevents errors before submission.

![Consultation booking wireframe](docs/wireframe-consultation-booking.png)

## Tools and methods

- **Figma** for the user journey map and wireframes
- **INVEST criteria** for user stories
- **Traceability matrix** linking requirement categories, user stories and business pain points
- **Accessibility and mobile-first design** (WCAG 2.1 AA, responsive layout, 44px touch targets)

## Repository structure

```
Managing-Software-Engineering-Project/
├── README.md
├── docs/
│   ├── Meeting_Lilys_Requirements.pdf   # Full report (requirements, journey, wireframes)
│   ├── user-journey-map.png             # Figma export, Wedding Sarah persona
│   ├── wireframe-landing-page.png
│   └── wireframe-consultation-booking.png
```

## What I learned

Systematic user research and requirements management can address real operational problems. The interview with Lily exposed pain points in inventory, delivery scheduling and event coordination, and those shaped the journey map, the functional and non-functional requirements, and finally the wireframes.

## Related Quantic work

This project belongs to the Managing Software Engineering block of the MSSE program. The same requirements-first approach carries into the later software design, testing and capstone projects.
