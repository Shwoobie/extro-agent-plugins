# Extro Trip Planner — preview release

Connects to https://extroapp.com/mcp and supplies a `plan-trip` skill. Guest creation requires no Extro account. Host permissions still apply; private-account operations require OAuth. Read https://extroapp.com/developers/mcp/create-guest-plans for data requirements and limits.

Ask: “Create a shareable three-day New York trip plan with restaurants, art, and cocktail bars.” Expect a real Extro link, a concise itinerary, booking caveats, and its expiration date.

This is a source package, not a marketplace-approved listing. No API key is bundled. It does not make bookings or automatically publish guides.

Install: `claude plugin install extro-trip-planner --marketplace Shwoobie/extro-agent-plugins`

[Privacy](https://extroapp.com/privacy) · [Terms](https://extroapp.com/terms)

## Data handling

The Extro MCP receives structured recommendations and plan details supplied by the agent. It stores the plan and recommendations on Extro's hosted backend. Unclaimed guest plans stop resolving after seven days; that is an access expiration, not a promise to delete all underlying records. Recommendation records and claimed plans can be retained longer than 30 days. Avoid sensitive personal data; use random session identifiers. The returned claim link should be shared only with the intended traveler.

When researching, the skill can use the host client's web search and browsing tools. The configured search provider and the public websites visited receive those search queries or requests under the host client's policies. No separate search credential is bundled. Only verified recommendation and plan data is sent to Extro through the declared connector. This plugin does not book travel or purchase tickets.
