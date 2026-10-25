# PM101 - Staymint cancellation flow

Product Management (PM101) mid-course group assignment, Masters Union: the hotel-cancellation experience for Staymint, an Android hotel-booking app built on Agoda's APIs.

Live prototype: https://staymint-prototype.vercel.app

## In this repo

| File | What it is |
| --- | --- |
| `PM101_Staymint_Cancellation_Wireframes_v5.pptx` | Final 14-slide submission deck (editable source) |
| `PM101_Staymint_Cancellation_Wireframes_v5.pdf` | The same deck as a PDF (rendered with LibreOffice, so fonts may differ slightly from Google Slides) |
| `PM101_Staymint_Flow_Diagrams_v5.pdf` | The four flow diagrams on their own (deck slides 4-7) |
| `staymint-prototype.html` | The clickable prototype as a single self-contained file - open in any browser, or use the live link above |
| `problem-statement.md` | The assignment brief, verbatim |

## What the deck covers

- A 2-page product note with the reasoning, the India refund problem size and the hotel room-night point, each with cited sources (source page at the end of the deck)
- The customer cancellation journey as a swimlane, plus a matching technical shadow showing API calls and data handoffs
- 5 wireframe screens, each with Designer (UI/UX), Developer (API usage) and Business notes
- A clickable prototype with reviewer demo scenarios

## Stated assumptions

- Partner Fulfillment model: the customer books, pays and cancels inside Staymint; Agoda owns policy, refund amount and the cancellation outcome
- Booking retrieval and cancellation APIs are enabled for the integration
- API cancellation works only until 1 day before check-in; outside that window the app routes to a prefilled support request
- Agoda does not document refund timing, refund method or notifications, so the app never claims money has arrived
- Booking-time Search API context (freeCancellation, freeCancellationDate, cancellationPolicy) is stored as a snapshot and shown as display-only during cancellation
