---
api_key_in: []
api_specs:
- filename: uplimit-organization-openapi-original.yml
  format: yaml
  label: Uplimit Organization API
  slug: uplimit-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplimit/refs/heads/main/openapi/uplimit-organization-openapi-original.yml
auth_types:
- http-bearer
description: ''
kind: authentication
layout: security
method: derived
name: Uplimit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uplimit secures its APIs with http-bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uplimit
provider_slug: uplimit
scheme_count: 1
schemes:
- applied: all operations (per-operation security)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/uplimit-organization-openapi-original.yml
  type: http
slug: uplimit-authentication
source_filename: uplimit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/uplimit-organization-openapi-original.yml\ndocs: https://github.com/uplimit/api-clients/blob/main/go-client/README.md\nsummary:\n  types: [http-bearer]\n  notes: Every operation on the Uplimit Organization API requires an\n    organization API token sent as an HTTP Bearer token. The go-client README\n    documents HTTP Bearer token authentication; GET /v1/Healthcheck validates\n    the key and returns the organization id/name (403 on a bad key). Tokens are\n    issued by Uplimit to Enterprise customers (no self-serve key portal was\n    found). Learner-facing SSO (SAML / OAuth2 identity binding) is managed via\n    POST /v1/AddUserAuthenticationMethod and is separate from API auth.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    applied: all operations (per-operation security)\n    sources: [openapi/uplimit-organization-openapi-original.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uplimit/refs/heads/main/authentication/uplimit-authentication.yml
summary_line: http-bearer · 1 scheme
tags:
- Company
- Future Of Work
- Learning
- Education
- Training
- Artificial Intelligence
- Corporate Training
---
