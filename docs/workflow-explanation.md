# Workflow Explanation

## Business problem
AI evaluation teams can receive large volumes of scores. Manual validation creates repetitive work and inconsistent routing.

## Automation
The workflow receives a webhook, validates required fields and score ranges, calculates the average, and routes the evaluation to PASS or HUMAN REVIEW.

## Why n8n
n8n provides visual workflow orchestration and can connect APIs, databases, messaging services and AI tools.

## Production version
A production workflow could add PostgreSQL persistence, reviewer notifications, dashboards and an LLM-based secondary evaluation layer.

## Skills demonstrated
Webhook/API handling · Data validation · Conditional routing · Workflow design · AI operations thinking.