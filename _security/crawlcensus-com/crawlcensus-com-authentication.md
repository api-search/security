---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Crawl Census Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crawl Census declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Crawl Census
provider_slug: crawlcensus-com
scheme_count: 2
schemes:
- description: Existing accounts hold an API key. Send it as a bearer token on every request. There is no query-string form, so keys do not end up in logs and referrers.
  header: Authorization
  issuance: New keys are not being issued; the tiers that came with one were withdrawn.
  key_prefix_example: cc_live_
  scheme: bearer
  scope: A key is scoped to one account. Rotating a key from the dashboard invalidates the previous one immediately.
  type: http
- description: Every read endpoint works unauthenticated (240 requests per hour per IP per the API page). POST /api/v1/scan and POST /api/v1/preflight also work without a key.
  type: none
slug: crawlcensus-com-authentication
source_filename: crawlcensus-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://crawlcensus.com/api\ndocs: https://crawlcensus.com/api\nname: Crawl Census authentication\nschemes:\n- type: http\n  scheme: bearer\n  header: Authorization\n  description: Existing accounts hold an API key. Send it as a bearer token on every request. There is no query-string form, so keys do not end up in logs and referrers.\n  key_prefix_example: cc_live_\n  scope: A key is scoped to one account. Rotating a key from the dashboard invalidates the previous one immediately.\n  issuance: New keys are not being issued; the tiers that came with one were withdrawn.\n- type: none\n  description: Every read endpoint works unauthenticated (240 requests per hour per IP per the API page). POST /api/v1/scan and POST /api/v1/preflight also work without a key.\nnote: No OAuth, no scopes. The API page example key is \"cc_live_9f2a7c41d8b34e6f\" (documentation sample, recorded only as the cc_live_ prefix).\n"
source_yaml_url: https://artifacts.apis.io/crawlcensus-com/authentication/crawlcensus-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI Crawlers
- Robots.txt
- SEO
- Web Measurement
- Open Data
- Llms.txt
- MCP
---
