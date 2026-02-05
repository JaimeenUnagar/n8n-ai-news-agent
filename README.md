# n8n AI News Agent – Domain Specific Slack Alerts

This project implements an automated AI-powered news monitoring system using n8n.

The workflow:
- ingests live RSS feeds
- normalizes and cleans heterogeneous news sources
- deduplicates articles
- classifies content into finance, tech and sports domains
- routes articles to domain-specific AI agents
- generates short summaries and impact statements
- sends alerts to Slack channels

## Architecture

RSS → Normalize → Dedupe → Domain Classifier → AI Agent → Slack

Each domain (finance, tech, sports) uses a separate AI agent with domain-specific prompting.

## Features

- Multi-source ingestion
- Schema normalization
- URL-based deduplication
- Rule-based domain classification
- Domain-specific AI summarization
- Slack delivery
- Rate limiting per domain

## Files

- `News Ingest – Day 1.json` – n8n workflow export

## How to run

1. Import the JSON workflow into n8n.
2. Configure:
   - Slack credentials
   - OpenAI credentials
3. Run the workflow manually or using the schedule trigger.

