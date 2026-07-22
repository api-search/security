---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ns1 Authentication
name_suffix: Authentication
oauth_flows: []
overview: NS1 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NS1
provider_slug: ns1
scheme_count: 1
schemes:
- description: 'NS1 API key issued from the portal (Account > Users & Teams > API Keys). Sent verbatim in the X-NSONE-Key header on every request to https://api.nsone.net/v1/. Verified live: an unauthenticated request to https://api.nsone.net/v1/zones returns HTTP 401.'
  in: header
  name: apiKey
  parameter_name: X-NSONE-Key
  sources:
  - github.com/ns1/ns1-python
  type: apiKey
slug: ns1-authentication
source_filename: ns1-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/ns1/ns1-python/blob/master/ns1/rest/resource.py\ndocs: https://ns1.com/api\nnotes: >-\n  NS1 (IBM NS1 Connect) authenticates every REST request with an API key sent in\n  the X-NSONE-Key request header. There is no OAuth2/OIDC surface; keys are issued\n  from the NS1 portal and can be scoped per team/user with granular permissions.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    parameter_name: X-NSONE-Key\n    description: >-\n      NS1 API key issued from the portal (Account > Users & Teams > API Keys).\n      Sent verbatim in the X-NSONE-Key header on every request to\n      https://api.nsone.net/v1/. Verified live: an unauthenticated request to\n      https://api.nsone.net/v1/zones returns HTTP 401.\n    sources: [github.com/ns1/ns1-python]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ns1/refs/heads/main/authentication/ns1-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Networking
- DNS
- Managed DNS
- Traffic Management
- DDI
- API
- Infrastructure
---
