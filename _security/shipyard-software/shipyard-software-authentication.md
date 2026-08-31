---
api_key_in:
- header
auth_types:
- apiKey
- http-basic
description: Authentication profile for the Clipper RFQ API, captured from the published API reference. The API is rate-limited; DEX aggregators obtain API credentials by contacting aggregators@shipyardsoftware.org. API v2 requires API key auth; API v1 still accepts a deprecated HTTP Basic scheme.
kind: authentication
layout: security
method: searched
name: Shipyard Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shipyard Software secures its APIs with apiKey and http-basic across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Shipyard Software
provider_slug: shipyard-software
scheme_count: 2
schemes:
- docs: https://docs.clipper.exchange/disclaimers-and-technical/integrating-with-clipper-rfq/api-reference/api-v2/overview
  in: header
  name: ApiKeyAuth
  notes: Required for all API v2 endpoints (blade-api.sushi.com) and supported on API v1 quote/sign endpoints.
  parameter: x-api-key
  status: current
  type: apiKey
- docs: https://docs.clipper.exchange/disclaimers-and-technical/integrating-with-clipper-rfq/api-reference/api-v1/overview
  name: BasicAuth
  notes: API v1 only — username:password credentials sent Base64-encoded in the Authorization header. Deprecated; the docs direct existing Basic users to request an API key. The v1 /rfq/pool endpoint currently only supports Basic Authentication (use Pool V2 for API key auth).
  scheme: basic
  status: deprecated
  type: http
slug: shipyard-software-authentication
source_filename: shipyard-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://docs.clipper.exchange/disclaimers-and-technical/integrating-with-clipper-rfq/api-reference/api-v2/overview\ndescription: >-\n  Authentication profile for the Clipper RFQ API, captured from the published\n  API reference. The API is rate-limited; DEX aggregators obtain API\n  credentials by contacting aggregators@shipyardsoftware.org. API v2 requires\n  API key auth; API v1 still accepts a deprecated HTTP Basic scheme.\nsummary:\n  types: [apiKey, http-basic]\n  api_key_in: [header]\ncredentials_contact: aggregators@shipyardsoftware.org\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  status: current\n  notes: >-\n    Required for all API v2 endpoints (blade-api.sushi.com) and supported on\n    API v1 quote/sign endpoints.\n  docs: https://docs.clipper.exchange/disclaimers-and-technical/integrating-with-clipper-rfq/api-reference/api-v2/overview\n- name: BasicAuth\n  type: http\n  scheme:\
  \ basic\n  status: deprecated\n  notes: >-\n    API v1 only — username:password credentials sent Base64-encoded in the\n    Authorization header. Deprecated; the docs direct existing Basic users to\n    request an API key. The v1 /rfq/pool endpoint currently only supports\n    Basic Authentication (use Pool V2 for API key auth).\n  docs: https://docs.clipper.exchange/disclaimers-and-technical/integrating-with-clipper-rfq/api-reference/api-v1/overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipyard-software/refs/heads/main/authentication/shipyard-software-authentication.yml
summary_line: apiKey/http-basic · 2 schemes
tags:
- Company
- Defi
- DEX
- Decentralized Exchange
- Cryptocurrency
- Trading
- Blockchain
- Web3
- Liquidity
- RFQ
---
