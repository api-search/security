---
api_key_in:
- unknown
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Soci Authentication
name_suffix: Authentication
oauth_flows: []
overview: SOCi secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SOCi
provider_slug: soci
scheme_count: 1
schemes:
- additional_parameters:
  - description: The customer's SOCi organization name, required alongside the key
    name: Organization Name
  - description: The customer's SOCi platform domain (e.g. app.meetsoci.com)
    name: Domain
  in: unknown
  issuance: Self-service inside the platform — a signed-in user generates a SOCi API Key from User Settings, reached from the menu at the top right of app.meetsoci.com.
  name: SOCi API Key
  parameter_name: unknown
  rotation_policy: not published
  scopes: none
  sources:
  - https://improvado.io/docs/soci
  - https://uni-select.meetsoci.com/docs/index.html
  type: apiKey
slug: soci-authentication
source_filename: soci-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://uni-select.meetsoci.com/docs/index.html\ndocs: https://uni-select.meetsoci.com/docs/index.html\ndocs_access: customer-only\nnote: >-\n  0-working/derive-authentication.py could not be used: SOCi publishes no OpenAPI,\n  so there are no securitySchemes to aggregate. The model below is assembled from\n  what SOCi's own surfaces state plus live anonymous probes of the API root.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - unknown\n  oauth2_flows: []\nschemes:\n- name: SOCi API Key\n  type: apiKey\n  in: unknown\n  parameter_name: unknown\n  issuance: >-\n    Self-service inside the platform — a signed-in user generates a SOCi API Key\n    from User Settings, reached from the menu at the top right of app.meetsoci.com.\n  additional_parameters:\n  - name: Organization Name\n    description: The customer's SOCi organization name, required alongside the key\n  - name: Domain\n    description: The customer's SOCi platform\
  \ domain (e.g. app.meetsoci.com)\n  rotation_policy: not published\n  scopes: none\n  sources:\n  - https://improvado.io/docs/soci\n  - https://uni-select.meetsoci.com/docs/index.html\noauth:\n  supported: false\n  evidence:\n  - url: https://app.meetsoci.com/.well-known/oauth-authorization-server\n    status: 404\n  - url: https://app.meetsoci.com/.well-known/openid-configuration\n    status: 404\nend_user_login:\n  url: https://app.meetsoci.com/admin/login\n  social_login_buttons:\n  - Google\n  - Apple\n  note: End-user platform sign-in only; not an API authorization surface.\ngaps:\n- The key placement (header vs query parameter) and the header name are not stated\n  on any public page — an integrator cannot write a first call without a customer\n  account.\n- No OAuth 2.0 / OIDC surface, so no delegated third-party authorization and no scoped\n  consent; every integration runs as a full-privilege user key.\n- No scope or permission model is published, so scopes/ is intentionally absent.\n\
  - No key-rotation, expiry or revocation policy is published.\nevidence:\n- url: https://uni-select.meetsoci.com/docs/index.html\n  status: 200\n  note: >-\n    Returns the SOCi application sign-in page (title \"SOCi - Social Media\n    Management... Solved\", an <h2>Sign In</h2> form) to anonymous visitors. Every\n    path under /docs/ returns the same 355,453-byte body, so the endpoint\n    reference itself is unreachable without a customer login.\n- url: https://app.meetsoci.com/api/v1/\n  status: 200\n  note: 'Live JSON error envelope returned anonymously: {\"status\":\"error\",\"error\":\"Invalid\n    API endpoint: v1\"}'\n- url: https://developers.meetsoci.com/\n  status: 302\n  note: Redirects to https://app.meetsoci.com/admin/login?redirect_to=L2RldmVsb3BlcnMv\n    (base64 \"/developers/\")\nx-evidence:\n  fetched: '2026-08-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soci/refs/heads/main/authentication/soci-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Marketing
- Local Marketing
- Multi-Location
- Reputation Management
- Listings Management
- Social Media Management
- Reviews
- Franchise
- Local SEO
---
