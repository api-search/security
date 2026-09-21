---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: webcrawlerapi-com-openapi.yml
  format: yaml
  label: WebCrawler API
  slug: webcrawler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webcrawlerapi-com/refs/heads/main/openapi/webcrawlerapi-com-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Webcrawlerapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: WebCrawlerAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WebCrawlerAPI
provider_slug: webcrawlerapi-com
scheme_count: 1
schemes:
- admin_key:
    note: The usage endpoint docs call for an "admin API key"; the spec declares the same ApiKeyAuth scheme with no scope distinction.
    required_for:
    - GET /v2/organization/usage
    source: https://webcrawlerapi.com/docs/api/organization/usage
  description: 'Docs: "Webcrawler API uses Bearer Token authentication scheme. You need to include the API key in the Authorization header" - Authorization: Bearer <API key>. The Swagger document models this as an apiKey scheme named Authorization with description "API key for authentication. Format: Bearer {api_key}" rather than as http/bearer; the wire format is identical. Applied per operation on 23 of 24 operations; GET /ping is anonymous.'
  failure:
    body: '{"error":"Unauthorized","message":"No Authorization header. Read the docs: https://webcrawlerapi.com/docs/access-key"}'
    docs_example: '{"error": "Unauthorized"}'
    observed: 2026-09-19 on POST /v1/crawl without a header
    status: 401
  format: Bearer {api_key}
  in: header
  key_management:
    default_key: true
    individual_revocation: true
    keys_per_organization: 20
    named_keys: true
    regenerate: at any time from the dashboard
    source: https://webcrawlerapi.com/changelog/2026-03-29-multiple-api-keys
  name: ApiKeyAuth
  obtain: Sign up at https://dash.webcrawlerapi.com/sign-up (no credit card), then copy a key from https://dash.webcrawlerapi.com/access.
  parameter: Authorization
  sdk_env_vars:
    claude_code_skill: WEBCRAWLERAPI_API_KEY
    cli: stored via `webcr auth set`
    mcp_server: WEBCRAWLER_API_KEY
  sources:
  - https://webcrawlerapi.com/docs/access-key
  - openapi/webcrawlerapi-com-openapi.yml
  type: apiKey
slug: webcrawlerapi-com-authentication
source_filename: webcrawlerapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://webcrawlerapi.com/docs/access-key + openapi/_original/webcrawlerapi-com-swagger.json (securityDefinitions.ApiKeyAuth)\n  + live unauthenticated 401 from api.webcrawlerapi.com observed 2026-09-19 + changelog 2026-03-29 (multiple API\n  keys)\ndocs: https://webcrawlerapi.com/docs/access-key\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  style: Bearer token carrying a static API key\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: Bearer {api_key}\n  description: 'Docs: \"Webcrawler API uses Bearer Token authentication scheme. You need to include the API key in\n    the Authorization header\" - Authorization: Bearer <API key>. The Swagger document models this as an apiKey scheme\n    named Authorization with description \"API key for authentication. Format: Bearer {api_key}\" rather than as http/bearer;\n\
  \    the wire format is identical. Applied per operation on 23 of 24 operations; GET /ping is anonymous.'\n  obtain: Sign up at https://dash.webcrawlerapi.com/sign-up (no credit card), then copy a key from https://dash.webcrawlerapi.com/access.\n  key_management:\n    keys_per_organization: 20\n    named_keys: true\n    default_key: true\n    individual_revocation: true\n    regenerate: at any time from the dashboard\n    source: https://webcrawlerapi.com/changelog/2026-03-29-multiple-api-keys\n  admin_key:\n    required_for:\n    - GET /v2/organization/usage\n    source: https://webcrawlerapi.com/docs/api/organization/usage\n    note: The usage endpoint docs call for an \"admin API key\"; the spec declares the same ApiKeyAuth scheme with\n      no scope distinction.\n  failure:\n    status: 401\n    body: '{\"error\":\"Unauthorized\",\"message\":\"No Authorization header. Read the docs: https://webcrawlerapi.com/docs/access-key\"}'\n    observed: 2026-09-19 on POST /v1/crawl without a\
  \ header\n    docs_example: '{\"error\": \"Unauthorized\"}'\n  sdk_env_vars:\n    mcp_server: WEBCRAWLER_API_KEY\n    claude_code_skill: WEBCRAWLERAPI_API_KEY\n    cli: stored via `webcr auth set`\n  sources:\n  - https://webcrawlerapi.com/docs/access-key\n  - openapi/webcrawlerapi-com-openapi.yml\nscopes: null\nscopes_note: No OAuth, no scopes; the only privilege distinction documented is the admin key for usage statistics.\nguidance: Keep the key server-side (docs warn against client-side code and public repos). Content URLs on data.webcrawlerapi.com\n  returned inside job items are fetched WITHOUT the key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webcrawlerapi-com/refs/heads/main/authentication/webcrawlerapi-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web Scraping
- Web Crawling
- Data Extraction
- Markdown
- AI Agents
- LLM
- RAG
- Web Feeds
- Change Detection
- Structured Data
- MCP
- A2A
- agent-native
---
