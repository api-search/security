---
api_key_in:
- header
auth_types:
- apiKey
- requestSignature
description: ''
kind: authentication
layout: security
method: searched
name: Telenav Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telenav secures its APIs with apiKey and requestSignature across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Telenav
provider_slug: telenav
scheme_count: 3
schemes:
- description: Telenav assigned API key, sent on every request.
  in: header
  name: x-tn-api_key
  parameter: x-tn-api_key
  type: apiKey
- description: Per-request API signature computed as apikey + ":" + timestamp + ":" + SHA256(apikey + ":" + timestamp + ":" + apisecret), where timestamp is UTC seconds. The docs include a sample Postman pre-request script for generating it.
  in: header
  name: x-tn-api_signature
  parameter: x-tn-api_signature
  type: apiKey
- description: Unique device identifier header, common to all endpoints.
  in: header
  name: x-tn-deviceid
  parameter: x-tn-deviceid
  type: apiKey
slug: telenav-authentication
source_filename: telenav-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.telenav.com/entity-rest/common.html\ndocs: https://docs.telenav.com/entity-rest/common.html#authentication\nnotes: >-\n  Telenav publishes no OpenAPI, so this profile is captured from the Entity\n  Service REST documentation rather than derived from securitySchemes. The\n  API uses a Telenav-assigned API key plus a per-request HMAC-style API\n  signature; credentials are provisioned to automotive partners (a free\n  six-month trial key/secret for the EU region is distributed through the\n  Telenav/nav-sdk-demo GitHub repository).\nsummary:\n  types: [apiKey, requestSignature]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: x-tn-api_key\n    type: apiKey\n    in: header\n    parameter: x-tn-api_key\n    description: Telenav assigned API key, sent on every request.\n  - name: x-tn-api_signature\n    type: apiKey\n    in: header\n    parameter: x-tn-api_signature\n    description: >-\n      Per-request\
  \ API signature computed as\n      apikey + \":\" + timestamp + \":\" + SHA256(apikey + \":\" + timestamp + \":\" + apisecret),\n      where timestamp is UTC seconds. The docs include a sample Postman\n      pre-request script for generating it.\n  - name: x-tn-deviceid\n    type: apiKey\n    in: header\n    parameter: x-tn-deviceid\n    description: Unique device identifier header, common to all endpoints.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telenav/refs/heads/main/authentication/telenav-authentication.yml
summary_line: apiKey/requestSignature · 3 schemes
tags:
- Mapping
- Navigation
- Location
- Search
- Automotive
- Connected Cars
- EV Charging
- Points of Interest
---
