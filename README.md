# attention-cockpit

A physical attention cockpit built on top of Stream Deck.

This project turns a Stream Deck into a persistent attention radar, combining:

- GTD (Getting Things Done)
- Calendar awareness
- Task tracking
- Alerting system
- Snooze / recheck workflows
- Environmental attention signaling (shoutbox concept)

---

## Concept

Instead of using the Stream Deck as a macro keyboard, this project redefines it as a:

PERSONAL OPERATIONS COCKPIT

Where you can:

- See what matters now
- Detect what requires attention
- Act on tasks and events
- Defer (snooze) or validate (recheck)
- Maintain continuous situational awareness

---

## Goals

- Provide an always-on attention interface
- Reduce reliance on OS notifications
- Centralize tasks, events, and alerts
- Enable controlled deferral (snooze)
- Support verifiable completion (recheck)
- Serve as a physical interface layer for future systems (e.g. PromptSync)

---

## MVP Scope (v0)

- Clock (always visible)
- Next calendar event
- Next task
- Overdue detection
- Alert signaling (color/blink)
- Basic snooze
- Manual completion/reset
- Local persistence

---

## Architecture

The system is built around 4 core components:

Connectors -> Engine -> Event Bus -> Renderers

### Connectors
Read external data (calendar, tasks, etc.)

### Engine
Applies rules and maintains system state

### Event Bus
Distributes updates internally

### Renderers
Display state and handle user interaction (Stream Deck)

---

## Current Interface

Primary device:
- Stream Deck (initial target)

Future possibilities:
- LED matrix display
- Web dashboard
- DIY hardware (corporate-safe environments)

---

## Roadmap

### v0
- Local tasks
- Clock
- Basic rendering
- Simple alerts

### v1
- Full GTD layout
- Shoutbox
- Multi-zone cockpit

### v2
- Recheck / validation
- Alert reactivation
- Improved state logic

### v3
- Shared lists
- Smart home integration
- External event ingestion

---

## Setup

python -m venv .venv
activate virtual environment

pip install -e .

Run:

python -m attention_cockpit.main

---

## Philosophy

This is not just a productivity tool.

It is an attempt to externalize attention into a physical, persistent interface.

---

## License

TBD
