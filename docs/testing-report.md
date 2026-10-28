# Testing Report — PG Finder Smart Stay Assistant

## 1. Testing Overview

The PG Finder voice assistant was configured through the CallKaro dashboard and tested using its chat-testing interface. Audio testing is being used to evaluate spoken interaction and speech recognition.

## 2. Test Cases

| Test | Input or Scenario | Expected Behavior | Observed Result |
|---|---|---|---|
| Greeting | Start a conversation | Agent introduces itself and asks whether the user has time | Passed in chat test |
| Requirement collection | Boys' PG in Bhopal, budget ₹7,000/month | Agent records the city, PG preference, and budget | Passed in chat test |
| Follow-up question | User has not shared move-in date | Agent asks a relevant question | Passed in chat test |
| Multiple preferences | Single room, food included, six-month stay | Agent collects the additional preferences | Passed in chat test |
| Context retention | User has already provided the city and budget | Agent should not ask for those details again | Needs improvement; repetition occurred during chat testing |
| Unsupported listing request | User requests an actual PG address and phone number | Agent explains that verified listings are unavailable | Passed in chat test; no fabricated contact details were provided |
| Spoken interaction | User speaks through Test Audio | Agent recognizes speech and responds aloud | In progress |
| Closing | User confirms the final summary | Agent acknowledges and closes naturally | Passed in chat test |

## 3. Sample Test Scenario

**User requirements:**
- City: Bhopal
- PG preference: Boys' PG
- Monthly budget: ₹7,000
- Room preference: Single room
- Food preference: Food included
- Move-in: Next month
- Stay duration: Six months
- Preferred locality: Not specified

**Expected outcome:**

The assistant should collect these requirements, summarize them accurately, avoid asking answered questions again, and explain that it cannot verify specific properties without connected listing data.

## 4. Issues Identified

- The agent repeated a question about the city after the user had already provided it.
- Some responses were delayed or temporarily stalled during chat testing.
- Repeated confirmations should be reduced after the user confirms the summary.

## 5. Improvements

- Strengthen conversation-context retention.
- Ask only for missing information.
- Keep confirmations concise.
- Improve response continuity and reduce unnecessary pauses.
- Clearly distinguish verified listing information from unavailable data.

## 6. Current Limitations

Verified live PG listings, real-time availability, and booking functionality are not connected. The assistant must not invent property details or claim that a booking has been made.

## 7. Status

- Chat testing: Completed, with improvements identified.
- Audio testing: In progress.
- Final regression testing: Pending.

*Update this report after completing audio testing so that all recorded results accurately reflect the final agent behavior.*
