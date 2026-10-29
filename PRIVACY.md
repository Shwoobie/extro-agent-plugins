# Extro Trip Planner privacy notice

Updated October 29, 2026. This notice describes the Extro agent plugin and public guest-plan MCP workflow. It supplements Extro's application policy for this integration; the server storage and retention described here apply to plugin submissions.

## Information sent to Extro

When an agent calls Extro, Extro receives the tool arguments: destination and dates, plan title and description, event and place names, addresses or locations, source and image URLs, proposed times, recommendation notes, and any other supplied fields. These may reveal travel preferences or personal plans. Do not submit sensitive personal details, private home addresses, credentials, or information about children. Guest creation does not require your name, email, or Extro account. It uses random conversation and request identifiers.

The service also receives network requests and records operational information for security and reliability. Guest-plan records include hashed conversation and network identifiers, provider information, a request identifier and payload hash, and a hashed claim token. Hashing these identifiers does not make all associated information anonymous.

## Use and storage

Extro stores submitted plans, events and places in its hosted backend to create and display shareable lists, support retries, prevent abuse, deduplicate recommendations, and let a traveler claim a plan. Hosting and database service providers process this information to operate the service. Recommendation records may be reused across plans. Submit recommendations suitable for sharing rather than confidential itinerary details.

## Sharing and claim links

Anyone who has a working public plan URL can view its shared contents. The claim-enabled URL additionally allows a signed-in recipient to keep the plan; share it only with the intended traveler. Event and place details may have their own public pages. A guest plan is not a private vault. Extro does not make reservations or purchase tickets through this plugin.

## Retention

An unclaimed guest plan stops resolving after seven days. This is an access expiration, not automatic deletion of every stored record. Underlying recommendations and operational records may remain, and claimed plans remain associated with the traveler's account. These records can be retained longer than 30 days. Signing in and claiming the plan removes its guest expiration.

## Other services

Your AI provider handles your conversation and tool interactions under its own privacy policy. When the plugin's instructions use host-provided web search or browsing, the configured search provider and visited public websites receive the corresponding queries or requests. Public images and external links can cause your browser to contact those sites when viewed or opened. The plugin bundles no search-provider credentials and does not need access to email or browser cookies. The guest workflow does not perform anonymous social-link extraction.

## Choices and contact

You can decline tool calls in clients that offer confirmations, avoid sensitive inputs, or disconnect the plugin. Disconnecting does not itself delete previously stored plans. For access or deletion requests, contact Extro through the privacy contact listed at https://extroapp.com/privacy. Do not post claim links, credentials, or private plans in public GitHub issues. Connected-account operations additionally use Extro's account authorization controls and app settings.
