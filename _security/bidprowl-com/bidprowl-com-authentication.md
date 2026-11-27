---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bidprowl-com-comps-api-openapi.yml
  format: yaml
  label: BidProwl Comps API
  slug: bidprowl-com-comps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-comps-api-openapi.yml
- filename: bidprowl-com-export-api-openapi.yml
  format: yaml
  label: BidProwl Export API
  slug: bidprowl-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-export-api-openapi.yml
- filename: bidprowl-com-flip-score-api-openapi.yml
  format: yaml
  label: BidProwl Flip Score API
  slug: bidprowl-com-flip-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-flip-score-api-openapi.yml
- filename: bidprowl-com-listings-api-openapi.yml
  format: yaml
  label: BidProwl Listings API
  slug: bidprowl-com-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-listings-api-openapi.yml
- filename: bidprowl-com-sold-api-openapi.yml
  format: yaml
  label: BidProwl Sold API
  slug: bidprowl-com-sold-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-sold-api-openapi.yml
- filename: bidprowl-com-sources-api-openapi.yml
  format: yaml
  label: BidProwl Sources API
  slug: bidprowl-com-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-sources-api-openapi.yml
- filename: bidprowl-com-usage-api-openapi.yml
  format: yaml
  label: BidProwl Usage API
  slug: bidprowl-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-usage-api-openapi.yml
- filename: bidprowl-com-webhooks-api-openapi.yml
  format: yaml
  label: BidProwl Webhooks API
  slug: bidprowl-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: BidProwl Authentication
name_suffix: Authentication
oauth_flows: []
overview: BidProwl secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BidProwl
provider_slug: bidprowl-com
scheme_count: 1
schemes:
- description: API key (bp_live_...) from bidprowl.com/account/api-keys
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bidprowl-com-openapi.json
  type: http
slug: bidprowl-com-authentication
source_filename: bidprowl-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/bidprowl-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key (bp_live_...) from bidprowl.com/account/api-keys\n  sources:\n  - openapi/bidprowl-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/bidprowl-com/authentication/bidprowl-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Government
- Auctions
- Marketplace
- Data
- Search
---
