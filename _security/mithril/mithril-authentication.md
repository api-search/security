---
api_key_in:
- header
api_specs:
- filename: mithril-compute-openapi-original.json
  format: json
  label: Mithril Compute API
  slug: mithril-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-compute-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Mithril Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mithril secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mithril
provider_slug: mithril
scheme_count: 1
schemes:
- bearerFormat: fkey_<key>
  docs: https://docs.mithril.ai/compute-api/compute-api-reference/api-keys
  header: 'Authorization: Bearer fkey_<key>'
  name: MithrilAPIKey
  scheme: bearer
  sources:
  - openapi/mithril-compute-openapi-original.json
  type: http
slug: mithril-authentication
source_filename: mithril-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/mithril-compute-openapi-original.json\ndocs: https://docs.mithril.ai/compute-api/compute-api-reference/api-keys\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: MithrilAPIKey\n  type: http\n  scheme: bearer\n  bearerFormat: fkey_<key>\n  header: 'Authorization: Bearer fkey_<key>'\n  docs: https://docs.mithril.ai/compute-api/compute-api-reference/api-keys\n  sources:\n  - openapi/mithril-compute-openapi-original.json\noauth_identity:\n  note: >-\n    Separately, the Mithril console/CLI sign-in uses OAuth 2.0 / OIDC at\n    login.mithril.ai (authorization_code, client_credentials, refresh_token,\n    device_code grants; scopes openid, profile, email, offline_access). This is\n    account identity, not the API's request auth (which is the fkey_ bearer key).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/authentication/mithril-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- GPU Cloud
- AI Infrastructure
- Machine Learning
- Cloud Computing
- Compute
- Spot Instances
- Kubernetes
- GPU
---
