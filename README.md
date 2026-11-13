# Slaide – Presentations & Slides (Cursor plugin)

Connects Cursor to [Slaide](https://www.slaide.de), an AI presentation maker. Ask the agent to build, edit and export
PowerPoint slide decks, documents and Excel workbooks. Everything lands in your own Slaide library.

This repository contains only the connection (`mcp.json`) and the plugin manifest. The server is hosted by Slaide at
`https://app.slaide.de/api/mcp` (Streamable HTTP).

## Setup

1. Install the plugin.
2. Cursor opens Slaide's sign-in page the first time a Slaide tool is used. Sign in with your Slaide account (a free
   account is enough) and press **Allow**. There is no token or API key to copy.
3. To disconnect: Slaide → Settings → Account → AI assistants. Access stops immediately.

## Tools

| Tool | What it does |
|---|---|
| `search_documents` | Lists your decks by title or recency |
| `get_document` | Reads the pages, speaker notes or cells of one of your documents |
| `create_document` | Starts a background job that builds a new presentation, document or workbook |
| `update_document` | Changes pages of an existing document (versioned, restorable in Slaide) |
| `get_job` | Reports progress and the result of a job |
| `export_document` | Produces a PowerPoint, PDF, Word, PNG or Excel file behind a private link that expires after 15 minutes |
| `cancel_job` | Stops a running job |

The connector cannot delete documents, buy anything, change a plan or reach other people's documents.

## Example prompts

- "Make a 10-slide presentation about remote work best practices for my team meeting."
- "Turn the attached PDF report into a 10-slide presentation and export it as PowerPoint."
- "In my Q3 Business Review deck, change the revenue on page 2 to 4.8 million euros. Change nothing else."

## Links

- Documentation: https://www.slaide.de/ai-assistants
- Privacy: https://www.slaide.de/privacy · Terms: https://www.slaide.de/terms
- Support: info@slaide.de

## License

The files in this repository are MIT-licensed (see `LICENSE`). Using the Slaide service is governed by the Slaide terms.
