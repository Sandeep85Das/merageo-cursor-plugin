# meraGEO AI Visibility for Cursor

Checks how ChatGPT, Claude and Gemini mention a website, right from Cursor.

- 0-100 AI visibility score for a domain
- Which models mention the site in answers to category questions
- The main issues found, mapped to page changes (llms.txt, FAQ, comparison pages)

The plugin connects Cursor to the hosted meraGEO MCP server at `https://merageo.com/api/mcp`. Sign-in uses OAuth on first use.

Tools: `get_ai_visibility_report`, `start_ai_visibility_scan`, `get_scan_status`, `get_profile`.

More at https://merageo.com
