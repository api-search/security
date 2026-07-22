---
api_key_in:
- query
api_specs:
- filename: one-degree-openapi.yml
  format: yaml
  label: One Degree Resource Server API
  slug: one-degree-resource-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/one-degree/refs/heads/main/openapi/one-degree-openapi.yml
auth_types:
- apiKey
- custom-signature
description: ''
kind: authentication
layout: security
method: searched
name: One Degree Authentication
name_suffix: Authentication
oauth_flows: []
overview: One Degree secures its APIs with apiKey and custom-signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: One Degree
provider_slug: one-degree
scheme_count: 2
schemes:
- description: All requests require an api_key query parameter. Request a key at http://socialservicedata.org/api/get-key/
  in: query
  name: apiKeyAuth
  parameter: api_key
  sources:
  - openapi/one-degree-openapi.yml
  type: apiKey
- applies_to:
  - POST
  - PUT
  - DELETE
  description: 'Write requests must include two additional headers: 1deg-Date (an ISO 8601 UTC timestamp, accepted within a 60-second window) and 1deg-Signature (a request signature). The signature is an HMAC-SHA256 chain: (1) HMAC-SHA256 hex digest of the request body keyed by the API secret token; (2) HMAC-SHA256 hex digest of the 1deg-Date timestamp keyed by the step-1 digest; (3) SHA-256 hex digest of the step-2 result.'
  docs: https://github.com/1deg/resource-server-api-docs/blob/main/docs/request-signatures.md
  headers:
  - description: ISO 8601 UTC timestamp (YYYY-MM-DDTHH:mm:ssZ), no milliseconds or timezone offset.
    name: 1deg-Date
  - description: Hexadecimal HMAC-SHA256 request signature authenticating the sender.
    name: 1deg-Signature
  name: requestSignature
  type: custom
slug: one-degree-authentication
source_filename: one-degree-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/one-degree-openapi.yml\ndocs: https://github.com/1deg/resource-server-api-docs/blob/main/docs/requests.md\nsummary:\n  types:\n  - apiKey\n  - custom-signature\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: >-\n    All requests require an api_key query parameter. Request a key at\n    http://socialservicedata.org/api/get-key/\n  sources:\n  - openapi/one-degree-openapi.yml\n- name: requestSignature\n  type: custom\n  applies_to:\n  - POST\n  - PUT\n  - DELETE\n  description: >-\n    Write requests must include two additional headers: 1deg-Date (an ISO 8601 UTC timestamp,\n    accepted within a 60-second window) and 1deg-Signature (a request signature). The signature is\n    an HMAC-SHA256 chain: (1) HMAC-SHA256 hex digest of the request body keyed by the API secret\n    token; (2) HMAC-SHA256 hex digest of the 1deg-Date timestamp keyed by the\
  \ step-1 digest;\n    (3) SHA-256 hex digest of the step-2 result.\n  headers:\n  - name: 1deg-Date\n    description: ISO 8601 UTC timestamp (YYYY-MM-DDTHH:mm:ssZ), no milliseconds or timezone offset.\n  - name: 1deg-Signature\n    description: Hexadecimal HMAC-SHA256 request signature authenticating the sender.\n  docs: https://github.com/1deg/resource-server-api-docs/blob/main/docs/request-signatures.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-degree/refs/heads/main/authentication/one-degree-authentication.yml
summary_line: apiKey/custom-signature · 2 schemes
tags:
- Company
- Nonprofit
- Social Services
- Community Resources
- Human Services
- Public Benefit
- Housing
- Open Data
- Civic Tech
- API
---
