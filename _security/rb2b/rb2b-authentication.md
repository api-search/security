---
api_key_in: []
auth_types:
- apiKey
description: Both RB2B REST surfaces authenticate with a single static account API key sent in a custom Api-Key request header. There is no OAuth 2.0, no OIDC, no bearer scheme, no HMAC request signing, no mutual TLS, and no scope model — one key grants the whole surface for the account it belongs to. RB2B publishes no OpenAPI, so this profile is read from the provider's documentation and its own shipped client rather than derived from securitySchemes.
kind: authentication
layout: security
method: searched
name: Rb2B Authentication
name_suffix: Authentication
oauth_flows: []
overview: RB2B secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RB2B
provider_slug: rb2b
scheme_count: 1
schemes:
- applies_to:
  - https://api.rb2b.com/api/v1
  - https://app.rb2b.com/api/v1
  description: Static per-account API key. The same header name is used on both the Identity/Enrichment API (api.rb2b.com) and the OEM Partner API (app.rb2b.com), but the keys are issued by two separate accounts and are not interchangeable.
  in: header
  name: apiKeyHeader
  parameter_name: Api-Key
  type: apiKey
slug: rb2b-authentication
source_filename: rb2b-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://support.rb2b.com/en/articles/12880800-using-the-rb2b-oem-program-api-webhook-guide\n  (OEM header table), the published @rb2b/rb2b-apis-mcp client (dist/api.js sets\n  the Api-Key header), and live unauthenticated probes of both API hosts on\n  2026-08-12.\ndescription: >-\n  Both RB2B REST surfaces authenticate with a single static account API key sent\n  in a custom Api-Key request header. There is no OAuth 2.0, no OIDC, no bearer\n  scheme, no HMAC request signing, no mutual TLS, and no scope model — one key\n  grants the whole surface for the account it belongs to. RB2B publishes no\n  OpenAPI, so this profile is read from the provider's documentation and its own\n  shipped client rather than derived from securitySchemes.\nsummary:\n  types: [apiKey]\n  oauth2: false\n  oidc: false\n  scopes: false\n  mtls: false\n  request_signing: false\nschemes:\n  - name: apiKeyHeader\n    type: apiKey\n    in: header\n\
  \    parameter_name: Api-Key\n    description: >-\n      Static per-account API key. The same header name is used on both the\n      Identity/Enrichment API (api.rb2b.com) and the OEM Partner API\n      (app.rb2b.com), but the keys are issued by two separate accounts and are\n      not interchangeable.\n    applies_to:\n      - https://api.rb2b.com/api/v1\n      - https://app.rb2b.com/api/v1\ncredentials:\n  - surface: Identity / Enrichment API (API Partner Program)\n    base_url: https://api.rb2b.com/api/v1\n    where_issued: https://ui.api.rb2b.com — the API Partner Program console (signup at /signup)\n    account_note: >-\n      A standalone account with its own unified credit balance, operating\n      independently from the consumer RB2B platform at app.rb2b.com.\n    key_prefix: null\n    key_prefix_note: >-\n      RB2B does not document a key prefix. The API does validate key SHAPE\n      before authenticating — a malformed value returns\n      {\"error\":\"invalid_api_key_format\"\
  } rather than a generic 401 — but the\n      expected format is not published.\n    rotation: >-\n      Not documented for the Identity API. For the OEM key, RB2B tells partners\n      to contact support to regenerate if the key is exposed or a holder leaves\n      the organisation, and warns that dependent systems must then be updated.\n    storage_guidance: >-\n      The first-party MCP server stores the key at ~/.rb2b/config.json with file\n      mode 0600 (owner read/write only) and offers a set_api_key tool that\n      validates a replacement before writing it.\n  - surface: OEM Partner API (domain management + credit usage)\n    base_url: https://app.rb2b.com/api/v1\n    where_issued: https://app.rb2b.com/oem_dashboard — the API Key card, copied in plain text\n    account_note: OEM partner account; the key governs which domains RB2B will track.\n    key_prefix: null\n    rotation: Contact RB2B support to regenerate; update dependent systems afterwards.\nrequired_headers:\n  - {name:\
  \ Api-Key, value: \"<account api key>\", required: true}\n  - {name: Content-Type, value: application/json, required: true}\n  - {name: Accept, value: application/json, required: true, note: documented for the OEM API}\n  - {name: User-Agent, value: \"<any>\", required: true, note: \"documented as required in the OEM header table\"}\nobserved:\n  - probe: GET https://api.rb2b.com/api/v1/credits\n    date: '2026-08-12'\n    sent: no Api-Key header\n    http_status: 401\n    body: '{\"error\":\"missing_api_key\"}'\n  - probe: POST https://api.rb2b.com/api/v1/ip_to_company\n    date: '2026-08-12'\n    sent: 'Api-Key: <deliberately malformed value>'\n    http_status: 401\n    body: '{\"error\":\"invalid_api_key_format\"}'\n  - probe: GET https://app.rb2b.com/api/v1/domains\n    date: '2026-08-12'\n    sent: no Api-Key header\n    http_status: 401\n    body: '{\"error\":\"missing_api_key\"}'\n  - probe: GET https://app.rb2b.com/api/v1/credit_usage\n    date: '2026-08-12'\n    sent: no Api-Key\
  \ header\n    http_status: 401\n    body: '{\"error\":\"missing_api_key\"}'\n    response_headers_of_note:\n      strict-transport-security: max-age=31536000; includeSubDomains; preload\n      x-request-id: present (uuid v4)\n      x-frame-options: DENY\n      x-content-type-options: nosniff\n      content-security-policy: present\ngaps:\n  - No published key-format or prefix convention, despite the API validating format.\n  - No self-service key rotation documented for either surface.\n  - No scopes, no least-privilege or read-only key type.\n  - No OAuth 2.0 for partner/OEM delegation — an OEM partner holds a single account-wide key.\n  - Outbound webhooks carry no signature or shared secret (see asyncapi/rb2b-webhooks.yml).\ndocs:\n  - https://support.rb2b.com/en/articles/12880800-using-the-rb2b-oem-program-api-webhook-guide\n  - https://www.npmjs.com/package/@rb2b/rb2b-apis-mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rb2b/refs/heads/main/authentication/rb2b-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Identity Resolution
- Visitor Identification
- B2B Data
- Lead Generation
- Sales Intelligence
- Marketing
- Data Enrichment
- LinkedIn Enrichment
- Hashed Email
- Mobile Ad ID
- Firmographics
- Webhook
- Pixel
- AdTech
- Identity Graph
- MCP
---
