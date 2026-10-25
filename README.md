# PM101 - Staymint cancellation flow

Product Management (PM101) mid-course group assignment, Masters Union: the hotel-cancellation experience for Staymint, an Android hotel-booking app built on Agoda's APIs.

Live prototype: https://staymint-prototype.vercel.app

## In this repo

Already here: this README, `problem-statement.md` (the assignment brief, verbatim) and `staymint-prototype.html` (the clickable prototype as a single self-contained file - open in any browser, or use the live link above).

Being added now (upload in progress):

| File | What it is |
| --- | --- |
| `PM101_Staymint_Cancellation_Wireframes_v2.pptx` | Final 13-slide submission deck (editable source) |
| `PM101_Staymint_Cancellation_Wireframes_v2.pdf` | The same deck as a PDF |
| `PM101_Staymint_Flow_Diagrams.pdf` | The four flow diagrams on their own (slides 2-5) |
| `flow-1-customer-journey-part1.png`, `flow-2-customer-journey-part2.png` | Customer swimlane: Customer / Our app / Agoda |
| `flow-3-technical-shadow-part1.png`, `flow-4-technical-shadow-part2.png` | Technical shadow: Customer / Android UI / Our backend / Agoda API, same step IDs with the data passed per step |

## What the deck covers

- The customer cancellation journey as a swimlane, plus a matching technical shadow showing API calls and data handoffs
- 7 wireframe screens, each with Designer (UI/UX), Developer (API usage) and Business notes
- A 2-page product note with the reasoning and stated assumptions
- A clickable prototype with reviewer demo scenarios

## Stated assumptions

- Partner Fulfillment model: the customer books, pays and cancels inside Staymint; Agoda owns policy, refund amount and the cancellation outcome
- Booking retrieval and cancellation APIs are enabled for the integration
- API cancellation works only until 1 day before check-in; outside that window the app routes to a prefilled support request
- Agoda does not document refund timing, refund method or notifications, so the app never claims money has arrived
- Booking-time Search API context (freeCancellation, freeCancellationDate, cancellationPolicy) is stored as a snapshot and shown as display-only during cancellation
