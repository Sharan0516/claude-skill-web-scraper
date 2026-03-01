# claude-skill-web-scraper

A Claude Code skill that extracts structured data from any website into a CSV using the Playwright MCP browser.

## What it does
- Scrapes contacts, alumni, attendees, leads, or any records from any URL
- Handles login-gated sites (you log in manually, Claude does the rest)
- Pagination, infinite scroll, AJAX/SPA sites
- Resumable sessions — pick up where you left off
- Deduplication, error logging, post-processing
- Multi-search-term runs with merged output

## Works great for
- LinkedIn connections
- Alumni directories (MIT, Harvard, etc.)
- Conference attendee lists (Luma, Whova, Eventbrite)
- Any business or people directory

## Installation
```bash
# 1. Download the .skill file from Releases
# 2. Install it
mkdir -p ~/.claude/skills
unzip web-scraper-extractor.skill -d ~/.claude/skills/

# 3. Add Playwright MCP
claude mcp add playwright -- npx @playwright/mcp

# 4. Restart Claude Code, then say:
# "Set up the web scraper prerequisites"
```

## Usage
Just describe what you want in Claude Code:
- *"Extract all contacts from this URL into a CSV"*
- *"Scrape my LinkedIn connections into a spreadsheet"*
- *"Resume the scraping session from yesterday"*

## Requirements
- Claude Code
- Node.js
- Python 3
