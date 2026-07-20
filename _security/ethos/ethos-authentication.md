---
api_key_in:
- server-issued-session-token
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ethos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ethos secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ethos
provider_slug: ethos
scheme_count: 1
schemes:
- description: 'Token auth: a bearer token is generated from a partner''s API key and tied to an individual application session. Session information is stored server-side and used to hydrate subsequent API calls; Ethos can invalidate a token, and payloads are kept minimal (only the data required for a given call) to protect applicants'' personal information.'
  name: partnerBearerToken
  provisioning: Partner API key issued by Ethos; not self-service / not publicly documented.
  scheme: bearer
  sources:
  - https://www.ethos.com/tech-and-ethos/partnership-apis-at-ethos/
  type: http
slug: ethos-authentication
source_filename: ethos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.ethos.com/tech-and-ethos/partnership-apis-at-ethos/\ndocs: https://www.ethos.com/api/\nnote: >-\n  Ethos publishes no public OpenAPI for its partnership API (access is provisioned per partner),\n  so this profile is derived from Ethos's own published engineering description of the auth model\n  rather than from a machine-readable securityScheme.\nsummary:\n  types:\n  - http\n  api_key_in:\n  - server-issued-session-token\n  oauth2_flows: []\nschemes:\n- name: partnerBearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    Token auth: a bearer token is generated from a partner's API key and tied to an individual\n    application session. Session information is stored server-side and used to hydrate subsequent\n    API calls; Ethos can invalidate a token, and payloads are kept minimal (only the data required\n    for a given call) to protect applicants' personal information.\n  provisioning: Partner API\
  \ key issued by Ethos; not self-service / not publicly documented.\n  sources:\n  - https://www.ethos.com/tech-and-ethos/partnership-apis-at-ethos/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ethos/refs/heads/main/authentication/ethos-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Insurance
- Life Insurance
- Insurtech
- Underwriting
- Financial Services
- Estate Planning
- Partnership API
---
