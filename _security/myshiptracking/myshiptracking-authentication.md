---
api_key_in: []
api_specs:
- filename: myshiptracking-openapi.yml
  format: yaml
  label: MyShipTracking Vessel Position API
  slug: myshiptracking-vessel-position-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/openapi/myshiptracking-openapi.yml
- filename: myshiptracking-openapi.yml
  format: yaml
  label: MyShipTracking Vessels in Area API
  slug: myshiptracking-vessels-in-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/openapi/myshiptracking-openapi.yml
- filename: myshiptracking-openapi.yml
  format: yaml
  label: MyShipTracking Vessel Search API
  slug: myshiptracking-vessel-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/openapi/myshiptracking-openapi.yml
- filename: myshiptracking-openapi.yml
  format: yaml
  label: MyShipTracking Vessel Particulars API
  slug: myshiptracking-vessel-particulars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/openapi/myshiptracking-openapi.yml
- filename: myshiptracking-openapi.yml
  format: yaml
  label: MyShipTracking Port Calls API
  slug: myshiptracking-port-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/openapi/myshiptracking-openapi.yml
- filename: myshiptracking-openapi.yml
  format: yaml
  label: MyShipTracking ETA API
  slug: myshiptracking-eta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/openapi/myshiptracking-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: documented
name: Myshiptracking Authentication
name_suffix: Authentication
oauth_flows: []
overview: MyShipTracking secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MyShipTracking
provider_slug: myshiptracking
scheme_count: 2
schemes:
- description: 'API key issued from your MyShipTracking account page, passed as `Authorization: Bearer [example key]`. Register a free account at MyShipTracking.com, then generate your API Key and Secret Key on the account page. Each user may hold one trial key (2,000 coins, 10 days).'
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://api.myshiptracking.com/
  - https://api.myshiptracking.com/docs/account-info
  type: http
- description: The same API key may instead be passed in the `x-api-key` request header. Either Bearer or x-api-key is accepted on every endpoint.
  in: header
  name: x-api-key
  sources:
  - https://api.myshiptracking.com/
  - https://api.myshiptracking.com/docs/vessel-current-position-api
  type: apiKey
slug: myshiptracking-authentication
source_filename: myshiptracking-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://api.myshiptracking.com/ (Getting Started + per-endpoint docs)\nsummary:\n  types:\n  - apiKey\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API key issued from your MyShipTracking account page, passed as\n    `Authorization: Bearer [example key]`. Register a free account at\n    MyShipTracking.com, then generate your API Key and Secret Key on the account\n    page. Each user may hold one trial key (2,000 coins, 10 days).\n  in: header\n  sources:\n  - https://api.myshiptracking.com/\n  - https://api.myshiptracking.com/docs/account-info\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  name: x-api-key\n  description: >-\n    The same API key may instead be passed in the `x-api-key` request header.\n    Either Bearer or x-api-key is accepted on every endpoint.\n  sources:\n  - https://api.myshiptracking.com/\n  - https://api.myshiptracking.com/docs/vessel-current-position-api\n\
  notes: >-\n  Authentication is required on every call. Missing keys return ERR_NO_KEY (401)\n  and invalid keys return ERR_INVALID_KEY (401). Keys can be regenerated from the\n  account page. The Secret Key is issued alongside the API Key at registration.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/authentication/myshiptracking-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Vessel Tracking
- AIS
- Maritime
- Ship Tracking
- Real-Time Data
- Ships
- Port Calls
- Maritime Data
- Location
- Fleet Tracking
---
