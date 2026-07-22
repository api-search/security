---
api_key_in:
- header
api_specs:
- filename: tollbit-openapi.json
  format: json
  label: TollBit API
  slug: tollbit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tollbit/refs/heads/main/openapi/tollbit-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tollbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tollbit secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tollbit
provider_slug: tollbit
scheme_count: 3
schemes:
- description: Organization secret API key from the Developer Dashboard Access page. Used on management endpoints (tokens, rates, search, catalog, self-report, webhook history). Never send the API key to a publisher `tollbit.*` subdomain.
  in: header
  name: ApiKeyAuth
  parameter: TollbitKey
  sources:
  - openapi/tollbit-openapi.json
  - https://docs.tollbit.com/docs/quickstart
  type: apiKey
- description: One-time, cryptographically signed JWT (also referenced as `TollbitToken`) minted from the Tokens API and presented on the Get Content endpoint, paired with a `User-Agent` carrying your AgentID. Single-use; 5-minute expiry.
  in: header
  name: ApiKeyAuth_
  parameter: Tollbit-Token
  sources:
  - openapi/tollbit-openapi.json
  - https://docs.tollbit.com/docs/content
  type: apiKey
- description: Bearer JWT signed by TollBit, scoped to a specific publisher subdomain and the permissions granted. Obtained via the TokensService Create Content Access Token call, then sent in the `Authorization` header when fetching content directly from a `tollbit.<domain>` front door.
  name: SubdomainAccessToken
  scheme: Bearer
  sources:
  - openapi/tollbit-openapi.json
  - https://docs.tollbit.com/docs/quickstart
  type: http
slug: tollbit-authentication
source_filename: tollbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/tollbit-openapi.json\ndocs: https://docs.tollbit.com/docs/quickstart\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  overview: >-\n    TollBit uses two layers of auth. Management/discovery calls (search, rates,\n    tokens, catalog, self-report, webhook history) authenticate with an\n    organization API key in the `TollbitKey` header (obtained from the Access\n    page of the Developer Dashboard at hack.tollbit.com). Actual content\n    retrieval never uses the API key directly: you first mint a cryptographically\n    signed, single-use JWT via the Tokens API, then pass it in the `TollbitToken`\n    header (over the gateway) or as a `Bearer` token in the `Authorization`\n    header (against a publisher `tollbit.<domain>` subdomain), along with a\n    `User-Agent` that contains your registered AgentID. Tokens expire 5 minutes\n    after issuance and are invalidated on first use to defend against\
  \ replay and\n    man-in-the-middle attacks.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: TollbitKey\n  description: >-\n    Organization secret API key from the Developer Dashboard Access page. Used\n    on management endpoints (tokens, rates, search, catalog, self-report,\n    webhook history). Never send the API key to a publisher `tollbit.*`\n    subdomain.\n  sources:\n  - openapi/tollbit-openapi.json\n  - https://docs.tollbit.com/docs/quickstart\n- name: ApiKeyAuth_\n  type: apiKey\n  in: header\n  parameter: Tollbit-Token\n  description: >-\n    One-time, cryptographically signed JWT (also referenced as `TollbitToken`)\n    minted from the Tokens API and presented on the Get Content endpoint,\n    paired with a `User-Agent` carrying your AgentID. Single-use; 5-minute\n    expiry.\n  sources:\n  - openapi/tollbit-openapi.json\n  - https://docs.tollbit.com/docs/content\n- name: SubdomainAccessToken\n  type: http\n  scheme: Bearer\n  description: >-\n \
  \   Bearer JWT signed by TollBit, scoped to a specific publisher subdomain and\n    the permissions granted. Obtained via the TokensService Create Content\n    Access Token call, then sent in the `Authorization` header when fetching\n    content directly from a `tollbit.<domain>` front door.\n  sources:\n  - openapi/tollbit-openapi.json\n  - https://docs.tollbit.com/docs/quickstart\ntokens:\n  format: JWT\n  signing: 'ECDSA / ES256 (example header alg=ES256)'\n  single_use: true\n  expiry: 5 minutes after issuance\n  types:\n  - content\n  - crawl\n  claims_note: >-\n    Standard JWT claims (iss/sub/aud/exp/nbf/iat/jti) plus token type `tt`\n    (content|crawl) and an `x` extras container binding user agent (`x.ua`) and,\n    for content tokens, max price micros (`x.mpm`), currency (`x.cur`), license\n    type (`x.lt`), and license id (`x.lid`).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tollbit/refs/heads/main/authentication/tollbit-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Content Licensing
- Content Monetization
- AI Agents
- Agentic Web
- Search
- Bot Management
- Web Infrastructure
- Developer API
---
