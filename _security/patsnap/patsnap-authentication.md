---
api_key_in: []
api_specs:
- filename: patsnap-openapi-original.json
  format: json
  label: Patsnap Open Platform API
  slug: patsnap-open-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patsnap/refs/heads/main/openapi/patsnap-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Patsnap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Patsnap secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Patsnap
provider_slug: patsnap
scheme_count: 1
schemes:
- alt_query_param: apikey
  format: Bearer sk-...
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/patsnap-openapi-original.json
  type: http
slug: patsnap-authentication
source_filename: patsnap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/patsnap-openapi-original.json\ndocs: https://open.patsnap.com/devportal/guides/authentication\nsummary:\n  types:\n  - http\n  scheme: bearer\n  notes: >-\n    Patsnap Open Platform (Eureka) uses API-Key authentication. Every request must carry a\n    valid API key (keys are prefixed `sk-`). The key is passed as an HTTP bearer token\n    (`Authorization: Bearer YOUR_API_KEY`, recommended) or, less securely, as an `apikey`\n    query parameter. There is no OAuth token endpoint, client_id/client_secret, or refresh\n    flow. The same key model authenticates the hosted MCP servers.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer sk-...'\n  alt_query_param: apikey\n  sources:\n  - openapi/patsnap-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patsnap/refs/heads/main/authentication/patsnap-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Technology
- Patents
- Intellectual Property
- Innovation Intelligence
- Patent Search
- Life Sciences
- R&D
- Analytics
- Artificial Intelligence
---
