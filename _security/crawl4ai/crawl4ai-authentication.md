---
api_key_in: []
auth_types: []
description: 'Crawl4AI authenticates with bearer API keys on both hosted surfaces and with a server-minted JWT on the self-hosted Docker server. There is no OAuth on any API: the only OAuth in the product is GitHub/Google sign-in for the human dashboard, which issues no API token to third parties. No published OpenAPI declares these schemes — every field below is read from the provider''s own docs.'
kind: authentication
layout: security
method: searched
name: Crawl4Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crawl4AI declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Crawl4AI
provider_slug: crawl4ai
scheme_count: 3
schemes:
- alternate:
    format: sk_live_...
    header: x-api-key
    in: header
  api: Crawl4AI Cloud API
  format: Bearer sk_live_...
  header: Authorization
  id: gate-bearer
  in: header
  key_prefix: sk_live_
  obtain: Click "Get a key" at https://gate.crawl4ai.com/ — a 24-hour Play key is issued instantly with no signup; verify your email to keep it permanently.
  rotate: https://gate.crawl4ai.com/dashboard/
  scopes: none
  style: bearer
  type: apiKey
  verified:
    body_length: 0
    date: '2026-08-29'
    probe: POST https://gate.crawl4ai.com/scrape with no credential
    status: 401
- api: Crawl4AI Cloud v1 API
  env_var: CRAWL4AI_API_KEY
  header: X-API-Key
  id: v1-api-key
  in: header
  note: The v1 API on api.crawl4ai.com uses the X-API-Key header rather than the Authorization bearer of the gate surface. 401 is documented as "Missing X-API-Key header, invalid/expired key".
  obtain: https://gate.crawl4ai.com/dashboard/
  scopes: none
  type: apiKey
- api: Crawl4AI Self-Hosted Docker API
  docs: https://docs.crawl4ai.com/core/self-hosting/
  format: Bearer <token>
  header: Authorization
  id: selfhosted-jwt
  in: header
  note: Since 0.9.0 authentication is ON BY DEFAULT. With no CRAWL4AI_API_TOKEN the server binds 127.0.0.1 and prints a one-off local token; exposing it requires setting CRAWL4AI_API_TOKEN and sending a bearer on every request except GET /health. The JWT implementation changed in 0.9.0 and all pre-0.9.0 tokens were invalidated. Monitor mutations (POST /monitor/actions/*, /monitor/stats/reset) require an admin-scope principal.
  scopes:
  - admin
  style: bearer
  token_endpoint: POST /token
  type: http
slug: crawl4ai-authentication
source_filename: crawl4ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://gate.crawl4ai.com/llms.txt, https://gate.crawl4ai.com/docs,\n  https://github.com/unclecode/crawl4ai-cloud-sdk (endpoint + error reference),\n  https://docs.crawl4ai.com/core/self-hosting/\nprovider: Crawl4AI\nproviderId: crawl4ai\ndescription: >-\n  Crawl4AI authenticates with bearer API keys on both hosted surfaces and with a\n  server-minted JWT on the self-hosted Docker server. There is no OAuth on any\n  API: the only OAuth in the product is GitHub/Google sign-in for the human\n  dashboard, which issues no API token to third parties. No published OpenAPI\n  declares these schemes — every field below is read from the provider's own docs.\nschemes:\n  - id: gate-bearer\n    api: Crawl4AI Cloud API\n    type: apiKey\n    style: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer sk_live_...'\n    alternate:\n      in: header\n      header: x-api-key\n      format: 'sk_live_...'\n    key_prefix:\
  \ sk_live_\n    scopes: none\n    obtain: >-\n      Click \"Get a key\" at https://gate.crawl4ai.com/ — a 24-hour Play key is\n      issued instantly with no signup; verify your email to keep it permanently.\n    rotate: https://gate.crawl4ai.com/dashboard/\n    verified:\n      probe: 'POST https://gate.crawl4ai.com/scrape with no credential'\n      status: 401\n      body_length: 0\n      date: '2026-08-29'\n  - id: v1-api-key\n    api: Crawl4AI Cloud v1 API\n    type: apiKey\n    in: header\n    header: X-API-Key\n    scopes: none\n    env_var: CRAWL4AI_API_KEY\n    obtain: https://gate.crawl4ai.com/dashboard/\n    note: >-\n      The v1 API on api.crawl4ai.com uses the X-API-Key header rather than the\n      Authorization bearer of the gate surface. 401 is documented as \"Missing\n      X-API-Key header, invalid/expired key\".\n  - id: selfhosted-jwt\n    api: Crawl4AI Self-Hosted Docker API\n    type: http\n    style: bearer\n    in: header\n    header: Authorization\n    format:\
  \ 'Bearer <token>'\n    token_endpoint: 'POST /token'\n    scopes:\n      - admin\n    note: >-\n      Since 0.9.0 authentication is ON BY DEFAULT. With no CRAWL4AI_API_TOKEN the\n      server binds 127.0.0.1 and prints a one-off local token; exposing it requires\n      setting CRAWL4AI_API_TOKEN and sending a bearer on every request except\n      GET /health. The JWT implementation changed in 0.9.0 and all pre-0.9.0\n      tokens were invalidated. Monitor mutations (POST /monitor/actions/*,\n      /monitor/stats/reset) require an admin-scope principal.\n    docs: https://docs.crawl4ai.com/core/self-hosting/\ndashboard_sign_in:\n  type: oauth2\n  providers:\n    - GitHub (GET /v1/auth/github/start)\n    - Google (GET /v1/auth/google/start)\n  note: >-\n    Human sign-in to the Crawl4AI dashboard only. No authorization-code flow is\n    published for third-party API access, no /.well-known/oauth-authorization-server\n    is served (probed 404, 2026-08-29), and no scope vocabulary exists\
  \ — which is\n    why no scopes/ artifact is written for this provider.\nmtls: false\nopenid_connect: false\nkey_handling:\n  storage_guidance: >-\n    Terms of Service §3 makes the account holder responsible for all activity\n    under their keys and requires prompt notification of a compromised key.\n  env_vars:\n    - CRAWL4AI_KEY\n    - CRAWL4AI_URL\n    - CRAWL4AI_API_KEY\n    - CRAWL4AI_API_TOKEN\nfailure_modes:\n  - status: 401\n    meaning: Missing or invalid key\n  - status: 403\n    meaning: Plan does not allow this feature, or caller is not the resource owner\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crawl4ai/refs/heads/main/authentication/crawl4ai-authentication.yml
summary_line: 3 schemes
tags:
- AI Automation
- Web Crawling
- Web Scraping
- Data Extraction
- Search
- LLM Tooling
- Agents
- MCP
- Open-Source
---
