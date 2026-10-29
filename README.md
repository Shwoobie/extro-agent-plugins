# Extro Trip Planner

Turn verified events, restaurants, bars, and attractions into one visual trip plan you can open and share.

[Documentation](https://extroapp.com/developers/mcp) · [Guest plans](https://extroapp.com/developers/mcp/create-guest-plans) · [Privacy](https://extroapp.com/privacy) · [Terms](https://extroapp.com/terms)

## Install

### Claude Code

```sh
claude plugin marketplace add Shwoobie/extro-agent-plugins
claude plugin install extro-trip-planner@extro
```

Start a new session and use `/extro-trip-planner:plan-trip`, or ask for a shareable trip plan.

### Gemini CLI

```sh
gemini extensions install https://github.com/Shwoobie/extro-agent-plugins
```

Start a new session and check `/mcp` for Extro. This is a Gemini CLI extension, not a consumer Gemini app listing.

### Codex and ChatGPT

The Codex compatibility package is in `plugins/codex/extro-trip-planner`. The portable OpenAI submission package is in `plugins/openai/extro-trip-planner`. Vendor directory reviews are pending; no approval is claimed. Clients supporting custom remote MCP servers can connect to `https://extroapp.com/mcp` directly.

## Try it

“Create a shareable three-day New York trip plan with great food, art, and cocktail bars. Research current recommendations, use Extro, and return the actual plan link.”

## How it works

The agent verifies recommendations, sends complete structured data to Extro, and returns a real list link with a summary. Guest creation does not require an Extro account. Plans expire after seven days unless claimed by signing in from the returned link. Up to 20 recommendations per guest plan and three plans per conversation per day by default; live capabilities and service budgets apply. Host-client approval prompts still apply.

Guest plans do not run anonymous social-link extraction. Existing private lists and connected-account operations require OAuth. Extro coverage varies; agents can research and supply their own recommendations. Nothing books travel, buys tickets, or guarantees availability.

## Privacy and source

Only standalone plugin instructions, manifests, and branding assets are included here. No application backend or credentials are distributed. Do not put sensitive personal information into shared plans. Treat claim-enabled URLs as private traveler handoffs.

## Support

Report integration problems through this repository's Issues tab. Do not include credentials, claim tokens, or private itineraries.

## License

MIT covers the integration code and instructions. Extro branding remains Extro's; this license does not grant trademark rights or rights to the hosted service or application backend.

## Data handling

The Extro MCP receives structured recommendations and plan details supplied by the agent. It stores the plan and recommendations on Extro's hosted backend. Unclaimed guest plans stop resolving after seven days; that is an access expiration, not a promise to delete all underlying records. Recommendation records and claimed plans can be retained longer than 30 days. Avoid sensitive personal data; use random session identifiers. The returned claim link should be shared only with the intended traveler.

When researching, the skill can use the host client's web search and browsing tools. The configured search provider and the public websites visited receive those search queries or requests under the host client's policies. No separate search credential is bundled. Only verified recommendation and plan data is sent to Extro through the declared connector. This plugin does not book travel or purchase tickets.
