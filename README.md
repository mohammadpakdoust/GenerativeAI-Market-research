# GenAI Market Research Automation

A multi-agent workflow that separates **web research** from **analysis and synthesis** to produce structured market-research reports.

## Overview

The project uses specialized agents for two distinct responsibilities:

1. **Research Agent** — gathers current company, market, competitor, and industry information from web search.
2. **Analyst Agent** — synthesizes the collected material into a structured business report.

This separation makes the workflow easier to inspect and reason about than a single monolithic prompt.

## Output

The generated report can include:

- Executive summary
- Company and market overview
- Competitor analysis
- SWOT analysis
- Strategic observations and recommendations

## Architecture

```text
Company / domain
      ↓
Research Agent
      ↓
Web search results
      ↓
Analyst Agent
      ↓
Structured Markdown report
```

## Tech stack

- Python 3.11+
- CrewAI
- Google Gemini
- Serper Web Search
- YAML configuration
- uv

## Key implementation ideas

- Separate research and synthesis responsibilities
- Use external search for current information
- Keep API credentials in environment variables
- Generate reports in a consistent Markdown structure
- Keep agent configuration separate from application code

## Repository

https://github.com/mohammadpakdoust/GenerativeAI-Market-research

## Background

Built as an applied Generative AI project focused on orchestration, structured outputs, and practical research automation.
