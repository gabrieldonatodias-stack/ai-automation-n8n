# AI Evaluation Automation with n8n

A workflow automation project that receives AI evaluation scores, validates them, calculates an average quality score, and routes each record to PASS or human review.

## Workflow
Webhook → Validate & Score → Quality Check → PASS / HUMAN REVIEW

## Rules
- Scores must be between 1 and 5.
- Average >= 3.5 → PASS.
- Average < 3.5 → REVIEW.
- Invalid or incomplete input → REVIEW.

## Repository structure
ai-automation-n8n/
- workflows/ai-evaluation-quality.json
- examples/input.json
- examples/expected_output.json
- docs/workflow-explanation.md
- README.md

## How to use
1. Open n8n.
2. Import the workflow JSON.
3. Execute the webhook in test mode.
4. Send the example JSON payload.
5. Inspect the structured response.

No credentials are required.

## Production extensions
PostgreSQL storage · Slack/email alerts · LLM secondary evaluation · dashboards · external APIs

Synthetic portfolio workflow only; no client credentials or confidential data.
