---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Groupon publishes no anonymously-readable OpenAPI, so this profile is derived from what the live gateway itself says. Every path on api.groupon.com — the root, /v2/*, /graphql, /mcp, /.well-known/* — returns the identical response {"error":{"httpCode":401,"message":"''client_id'' is invalid"}}. The gateway therefore names its own credential: a client_id. No WWW-Authenticate header is returned, no OAuth or OpenID discovery document is served on any Groupon host, and no bearer-token challenge is issued, so this is a plain API-key scheme, not OAuth. Nothing about scopes, key issuance or rotation could be read: the developer portal that would document it (www.groupon.com/developers) is behind a Cloudflare managed bot challenge that returns 403 to every automated client, including the Internet Archive.'
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Groupon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Groupon declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Groupon
provider_slug: groupon
scheme_count: 2
schemes:
- description: 'Client identifier required on every request to the Groupon API gateway. Established by probe, not by documentation: the gateway rejects requests with the message "''client_id'' is invalid" and accepts nothing anonymously.'
  evidence:
  - body: '{"error":{"httpCode":401,"message":"''client_id'' is invalid"}}'
    fetched: '2026-09-04'
    http_status: 401
    url: https://api.groupon.com/v2/deals.json
  - fetched: '2026-09-04'
    http_status: 401
    note: An arbitrary client_id is rejected, confirming the value is validated server-side.
    url: https://api.groupon.com/v2/deals.json?client_id=test
  host: api.groupon.com
  id: groupon_client_id
  in: query
  name: client_id
  type: apiKey
- description: 'The Groupon Partner Network reporting APIs (Order, Deal, Division, Transaction, Taxonomy, Campaign, Ledger) took a clientId query parameter issued from the GPN Account Profile page. RECORDED FOR HISTORY ONLY: partner-api.groupon.com now returns Cloudflare 522 (origin unreachable) and the Groupon Partner Network was permanently closed on 2022-06-15.'
  evidence:
  - fetched: '2026-09-04'
    http_status: 522
    url: https://partner-api.groupon.com/
  - fetched: '2026-09-04'
    note: 'Third-party affiliate-platform documentation, quoted: "Groupon Partner Network permanently closed on June 15, 2022, Groupon is now available on CJ Affiliate." Names the API Key / Authentication token from the GPN Account Profile section. Cited because Groupon''s own GPN help pages are no longer served.'
    url: https://strackr.com/docs/groupon
  host: partner-api.groupon.com
  id: groupon_partner_client_id
  in: query
  name: clientId
  status: retired
  type: apiKey
slug: groupon-authentication
source_filename: groupon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://api.groupon.com/ (live 401 probe, 2026-09-04)\ndescription: >-\n  Groupon publishes no anonymously-readable OpenAPI, so this profile is derived\n  from what the live gateway itself says. Every path on api.groupon.com — the\n  root, /v2/*, /graphql, /mcp, /.well-known/* — returns the identical response\n  {\"error\":{\"httpCode\":401,\"message\":\"'client_id' is invalid\"}}. The gateway\n  therefore names its own credential: a client_id. No WWW-Authenticate header is\n  returned, no OAuth or OpenID discovery document is served on any Groupon host,\n  and no bearer-token challenge is issued, so this is a plain API-key scheme, not\n  OAuth. Nothing about scopes, key issuance or rotation could be read: the\n  developer portal that would document it (www.groupon.com/developers) is behind a\n  Cloudflare managed bot challenge that returns 403 to every automated client,\n  including the Internet Archive.\nschemes:\n  - id: groupon_client_id\n\
  \    type: apiKey\n    in: query\n    name: client_id\n    host: api.groupon.com\n    description: >-\n      Client identifier required on every request to the Groupon API gateway.\n      Established by probe, not by documentation: the gateway rejects requests\n      with the message \"'client_id' is invalid\" and accepts nothing anonymously.\n    evidence:\n      - url: https://api.groupon.com/v2/deals.json\n        http_status: 401\n        body: '{\"error\":{\"httpCode\":401,\"message\":\"''client_id'' is invalid\"}}'\n        fetched: '2026-09-04'\n      - url: https://api.groupon.com/v2/deals.json?client_id=test\n        http_status: 401\n        note: An arbitrary client_id is rejected, confirming the value is validated server-side.\n        fetched: '2026-09-04'\n  - id: groupon_partner_client_id\n    type: apiKey\n    in: query\n    name: clientId\n    host: partner-api.groupon.com\n    status: retired\n    description: >-\n      The Groupon Partner Network reporting APIs (Order,\
  \ Deal, Division,\n      Transaction, Taxonomy, Campaign, Ledger) took a clientId query parameter\n      issued from the GPN Account Profile page. RECORDED FOR HISTORY ONLY:\n      partner-api.groupon.com now returns Cloudflare 522 (origin unreachable) and\n      the Groupon Partner Network was permanently closed on 2022-06-15.\n    evidence:\n      - url: https://partner-api.groupon.com/\n        http_status: 522\n        fetched: '2026-09-04'\n      - url: https://strackr.com/docs/groupon\n        note: >-\n          Third-party affiliate-platform documentation, quoted: \"Groupon Partner\n          Network permanently closed on June 15, 2022, Groupon is now available on\n          CJ Affiliate.\" Names the API Key / Authentication token from the GPN\n          Account Profile section. Cited because Groupon's own GPN help pages are\n          no longer served.\n        fetched: '2026-09-04'\noauth2: false\nopenid_connect: false\nmutual_tls: false\nnotes:\n  - >-\n    No /.well-known/openid-configuration\
  \ or /.well-known/oauth-authorization-server\n    exists on any Groupon host — all probed 404 (www/apex) or 401 (api gateway) on\n    2026-09-04.\n  - >-\n    The Groupon Developer Platform 2.0 integrations (Bookable Appointments, Tours\n    and Attractions) are contracts Groupon CONSUMES: Groupon polls and calls the\n    partner's own endpoints. Their authentication is therefore configured per\n    partner and is not a Groupon-hosted scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groupon/refs/heads/main/authentication/groupon-authentication.yml
summary_line: 2 schemes
tags:
- Fortune 1000
- Local Commerce
- Marketplace
- E-Commerce
- Deals
- Bookings
- Reservations
- Travel
- Retail
---
