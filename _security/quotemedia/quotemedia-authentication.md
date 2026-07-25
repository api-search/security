---
api_key_in:
- query
auth_types:
- entitlement-id
- session-token
- credentials
description: ''
kind: authentication
layout: security
method: searched
name: Quotemedia Authentication
name_suffix: Authentication
oauth_flows: []
overview: QuoteMedia secures its APIs with entitlement-id, session-token, and credentials across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: QuoteMedia
provider_slug: quotemedia
scheme_count: 3
schemes:
- description: 'Every QMOD request requires a sales-provisioned Webmaster ID passed as a query parameter, with data entitlements bound to that ID. Verified live: requests without it return faultcode 0002 ("Webmaster ID is required"), and an unentitled ID returns faultcode 403 FORBIDDEN.'
  in: query
  name: webmasterId
  parameter: webmasterId
  surface: QuoteMedia OnDemand (QMOD) REST API
  type: apiKey
- description: QMod embeddable components authenticate via the loader with access managed by "domain, referrer, IP, or token-based controls" (per the public QMod support article); a session identifier is negotiated by the loader rather than embedded API keys.
  name: sid-session
  surface: QMOD widgets / OnDemand sessions
  type: session
- description: The first-party streamer SDKs (npm @quotemedia.com/streamer, Maven streamerclient-java-core, NuGet QuotemediaStreamerClient) connect with sales-provisioned credentials; no self-service key issuance exists.
  name: streamer-credentials
  surface: Streaming Data Feed API (WebSocket / Java / .NET clients)
  type: credentials
slug: quotemedia-authentication
source_filename: quotemedia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: >-\n  live probes of https://app.quotemedia.com/data 2026-07-22;\n  https://www.quotemedia.com/apifeeds;\n  https://support.quotemedia.com/support/solutions/articles/13000020415-qmod-the-future-of-financial-web-content\nsummary:\n  types: [entitlement-id, session-token, credentials]\n  api_key_in: [query]\n  oauth2_flows: []\nschemes:\n  - name: webmasterId\n    type: apiKey\n    in: query\n    parameter: webmasterId\n    surface: QuoteMedia OnDemand (QMOD) REST API\n    description: >-\n      Every QMOD request requires a sales-provisioned Webmaster ID passed as a\n      query parameter, with data entitlements bound to that ID. Verified live:\n      requests without it return faultcode 0002 (\"Webmaster ID is required\"),\n      and an unentitled ID returns faultcode 403 FORBIDDEN.\n  - name: sid-session\n    type: session\n    surface: QMOD widgets / OnDemand sessions\n    description: >-\n      QMod embeddable components\
  \ authenticate via the loader with access managed\n      by \"domain, referrer, IP, or token-based controls\" (per the public QMod\n      support article); a session identifier is negotiated by the loader rather\n      than embedded API keys.\n  - name: streamer-credentials\n    type: credentials\n    surface: Streaming Data Feed API (WebSocket / Java / .NET clients)\n    description: >-\n      The first-party streamer SDKs (npm @quotemedia.com/streamer, Maven\n      streamerclient-java-core, NuGet QuotemediaStreamerClient) connect with\n      sales-provisioned credentials; no self-service key issuance exists.\ndocs: https://quotemediasupport.freshdesk.com/support/home\nnotes: >-\n  No OAuth2/OIDC surface is published (no /.well-known/openid-configuration or\n  oauth-authorization-server on any host). Full authentication reference is\n  behind the entitlement-gated Freshdesk knowledge base; Quotestream Connect for\n  Developers is the self-service onboarding path for non-professional use.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quotemedia/refs/heads/main/authentication/quotemedia-authentication.yml
summary_line: entitlement-id/session-token/credentials · 3 schemes
tags:
- Financial
- Market Data
- Stocks
- Options
- Real-Time
- Streaming
- News
- Fundamentals
- Reference Data
---
