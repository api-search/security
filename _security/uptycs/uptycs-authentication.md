---
api_key_in: []
auth_types:
- http
description: Uptycs publishes no public API reference (per-customer docs live in-product on each https://{stack}.uptycs.io tenant), but the authentication model is documented publicly through the official Uptycs pack for Cortex XSOAR. Each API user downloads a credentials file from the Uptycs console containing an API key, API secret, the stack domain, and the customer ID. Clients mint a short-lived HS256 JWT (iss = API key, exp = now + 3600s, signed with the API secret) and send it as an Authorization Bearer token, along with an RFC 1123 date header, to https://{stack}.uptycs.io/public/api/customers/{customerId}.
kind: authentication
layout: security
method: searched
name: Uptycs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uptycs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uptycs
provider_slug: uptycs
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Self-signed HS256 JWT minted by the client from a per-user API key (claim iss) and API secret (signing key), expiring within one hour. Credentials are issued per user, per customer stack, from the Uptycs console (user profile > API keys). No OAuth 2.0 / OIDC surface is published.
  name: UptycsApiJwt
  scheme: bearer
  sources:
  - https://github.com/demisto/content/blob/master/Packs/Uptycs/Integrations/Uptycs/Uptycs.py
  type: http
slug: uptycs-authentication
source_filename: uptycs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/demisto/content/blob/master/Packs/Uptycs/Integrations/Uptycs/Uptycs.py\ndocs: https://xsoar.pan.dev/docs/reference/integrations/uptycs\ndescription: >-\n  Uptycs publishes no public API reference (per-customer docs live in-product\n  on each https://{stack}.uptycs.io tenant), but the authentication model is\n  documented publicly through the official Uptycs pack for Cortex XSOAR. Each\n  API user downloads a credentials file from the Uptycs console containing an\n  API key, API secret, the stack domain, and the customer ID. Clients mint a\n  short-lived HS256 JWT (iss = API key, exp = now + 3600s, signed with the API\n  secret) and send it as an Authorization Bearer token, along with an RFC 1123\n  date header, to https://{stack}.uptycs.io/public/api/customers/{customerId}.\nsummary:\n  types:\n    - http\n  schemes:\n    - bearer\n  bearer_format: JWT (HS256)\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n\
  \  - name: UptycsApiJwt\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Self-signed HS256 JWT minted by the client from a per-user API key\n      (claim iss) and API secret (signing key), expiring within one hour.\n      Credentials are issued per user, per customer stack, from the Uptycs\n      console (user profile > API keys). No OAuth 2.0 / OIDC surface is\n      published.\n    sources:\n      - https://github.com/demisto/content/blob/master/Packs/Uptycs/Integrations/Uptycs/Uptycs.py\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptycs/refs/heads/main/authentication/uptycs-authentication.yml
summary_line: http · 1 scheme
tags:
- Security
- Cybersecurity
- CNAPP
- XDR
- Cloud Security
- Endpoint Security
- Kubernetes Security
- Osquery
- Threat Detection
- Compliance
---
