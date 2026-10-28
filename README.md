# PG Finder – Smart Stay Assistant

An AI-powered voice assistant built using CallKaro to help users communicate their PG (paying guest) accommodation requirements through a natural conversation.

## Overview

Finding suitable PG accommodation can involve multiple questions about location, budget, room type, food preferences, and move-in date. PG Finder is designed to collect these requirements conversationally and organize them for follow-up.

The agent is configured and tested through the CallKaro dashboard.

## Features

- **Conversational voice interface:** Greets users and collects accommodation requirements.
- **Requirement collection:** Captures preferred city, gender preference, monthly budget, locality, room preference, food preference, move-in date, and intended stay duration.
- **Conversation context:** Uses previously shared information to guide follow-up questions.
- **Knowledge base:** Uses service information and FAQs to support responses.
- **Post-call analysis:** Extracts structured customer requirements, conversation summaries, call outcomes, and conversion information.
- **Responsible responses:** Avoids inventing PG addresses, phone numbers, prices, or availability when verified information is unavailable.

## Technology

- CallKaro voice-agent platform
- Configurable language model and speech processing
- Knowledge-base integration
- Structured post-call data extraction

## Example Conversation

**User:** I'm looking for a boys' PG in Bhopal with a monthly budget of ₹7,000.

**Assistant:** When are you planning to move in?

**User:** Next month. I'd prefer a single room with food included, and I plan to stay for six months.

The assistant is designed to gather the remaining requirements, summarize the user's preferences, and avoid claiming that a specific PG is available without verified listing data.

## Current Limitations

- Verified live PG listings and availability are not currently connected.
- The agent cannot guarantee a booking or provide verified contact details without a suitable data source.
- Live calling depends on the required phone-number and telephony configuration.
- This repository documents the project; the agent itself is configured on the CallKaro platform.

## Testing

The agent has been tested using the dashboard's chat-testing interface. Audio testing is being used to evaluate speech recognition, spoken responses, conversation continuity, and handling of unsupported requests.

Additional testing should verify that the agent does not repeatedly ask answered questions and does not fabricate accommodation details.

## Project Status

**Status:** Prototype configured; testing and documentation in progress.

## Demo

Demo video: To be added.

## Repository Contents

- `README.md` — Project overview, features, and limitations.
- `docs/system-prompt.md` — Agent prompt documentation.
- `docs/testing-report.md` — Test scenarios and observations.
- `knowledge-base/PG_Finder_Service_Information_and_FAQs.pdf` — Service information and FAQs used by the agent.

## Disclaimer

This is an accommodation-assistance prototype, not a verified PG listing marketplace. Users should independently verify property details, prices, availability, and contact information before making accommodation decisions.
