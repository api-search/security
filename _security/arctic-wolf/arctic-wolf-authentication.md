---
api_key_in: []
api_specs:
- filename: arctic-wolf-ticket-api-openapi.json
  format: json
  label: Arctic Wolf Ticket API
  slug: arctic-wolf-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arctic-wolf/refs/heads/main/openapi/arctic-wolf-ticket-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Arctic Wolf Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arctic Wolf secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arctic Wolf
provider_slug: arctic-wolf
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/arctic-wolf-ticket-api-openapi.json
  type: http
slug: arctic-wolf-authentication
source_filename: arctic-wolf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/arctic-wolf-ticket-api-openapi.json\ndocs: https://docs.arcticwolf.com/en/developer-and-oem/ticket-api/ticket-api-quick-start-guide/use-the-ticket-api\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_format: JWT\n  credential: Personal API Key\nnotes: >-\n  Arctic Wolf APIs (Ticket API, User API, Aurora Endpoint Defense API) authenticate\n  with a bearer JWT. Developers generate a Personal API Key in the Unified Portal\n  (portal.arcticwolf.com) under Organization Profile > Personal API Keys, then pass\n  it as a bearer token. Service endpoints are regional pods (US001/US002/US003,\n  EU001, AU001, CA001); select the pod that matches your organization. The Aurora\n  Endpoint Defense API additionally documents a short-lived access-token lifecycle\n  (tokens are single-use per request and valid for a few minutes).\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n \
  \ sources:\n  - openapi/arctic-wolf-ticket-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arctic-wolf/refs/heads/main/authentication/arctic-wolf-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Security Operations
- Threat Intelligence
- Ticketing
- Endpoint Security
- SOC
---
