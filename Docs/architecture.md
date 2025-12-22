# System Architecture

This system is built as an **event-driven autonomous agent** using n8n.

## Architectural Components

### 1. Trigger Layer
- Gmail Trigger detects new incoming emails

### 2. Perception Layer
- Email content and metadata are extracted
- Passed to the AI Agent for semantic understanding

### 3. Reasoning Layer
- LLM classifies intent
- Calendar availability is checked
- Goals are retrieved from Airtable

### 4. Decision Layer
- Rule-based switch routes execution
- Ensures deterministic safety

### 5. Action Layer
- Gmail Draft or Label nodes execute actions
- System completes loop without human input
docs/decision-logic.md
md
Copy code
# Decision Logic & Autonomy Boundaries

## Classification → Action Mapping

| Category       | Action |
|---------------|--------|
| SPAM          | Label only |
| PROMOTIONAL   | Label only |
| EDUCATIONAL   | Conditional reply |
| SPONSORSHIP   | Goal-aligned reply |
| IMPORTANT     | Immediate reply |

## Autonomy Controls
- No self-scheduling of meetings
- No financial commitments
- No irreversible actions

## Failure Handling
- If tools fail → fallback to labeling
- If context unavailable → conservative response
