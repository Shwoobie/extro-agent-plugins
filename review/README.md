# Extro reviewer walkthrough

The video is a captioned walkthrough of actual production MCP request/response evidence, not a recording of the ChatGPT interface. Run date: October 29, 2026. No Extro account, password, API key or OAuth sign-in is required for these eight public tools. Host-client confirmations still apply.

The five positive scenarios cover capabilities and types, published guides, public places/events, structured guest creation, and status/idempotent retry. The three negative scenarios cover link-only guest imports, oversized requests and unauthenticated private access. `results.json` records 12 actual tool calls. Claim-enabled URLs were removed from public evidence.

`sample-plan.json` contains a proposed November 6–8 New York itinerary with 10 sightseeing visits and 10 restaurant/bar options. Visits are clearly labeled personal suggestions, not organizer-announced events or bookings. For a new reviewer run, replace requestId and clientSessionId with random IDs once. On retries, preserve those IDs and the entire payload. Do not rotate identifiers to bypass limits. API replay checks were executed; natural-language host behavior is described as an expectation, not claimed as a completed ChatGPT test.

Guest links expire after seven days unless claimed. The example output may expire; case 4 returns a fresh valid link when rerun. Follow the new link from the tool result. No testing credentials are needed. Connect using Streamable HTTP at https://extroapp.com/mcp.

[Demo video](https://raw.githubusercontent.com/Shwoobie/extro-agent-plugins/main/review/extro-mcp-review.mp4) · [Sample input](sample-plan.json) · [Recorded results](results.json)
