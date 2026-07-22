---
api_key_in:
- header
auth_types:
- http
- apiKey
description: 'Muse Finance API authentication. Every request must carry TWO credentials: a JWT bearer token in the Authorization header AND a static API key in the x-api-key header. Partners are issued an API key, Client ID and Client Secret by Muse (via technical-support@getmymuse.com), then exchange those for a short-lived JWT through a designated token-exchange endpoint before calling the API.'
kind: authentication
layout: security
method: searched
name: Muse Finance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Muse Finance secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Muse Finance
provider_slug: muse-finance
scheme_count: 2
schemes:
- bearer_format: JWT
  description: Short-lived JWT obtained by exchanging the issued API key + Client ID + Client Secret at the designated token-exchange endpoint.
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - docs
  type: http
  value_prefix: 'Bearer '
- description: Static partner API key, issued by Muse Finance support.
  in: header
  name: apiKeyAuth
  parameter_name: x-api-key
  sources:
  - docs
  type: apiKey
slug: muse-finance-authentication
source_filename: muse-finance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api-docs.getmymuse.com/docs/authentication\ndocs: https://api-docs.getmymuse.com/docs/authentication\ndescription: >-\n  Muse Finance API authentication. Every request must carry TWO credentials: a\n  JWT bearer token in the Authorization header AND a static API key in the\n  x-api-key header. Partners are issued an API key, Client ID and Client Secret\n  by Muse (via technical-support@getmymuse.com), then exchange those for a\n  short-lived JWT through a designated token-exchange endpoint before calling\n  the API.\nsummary:\n  types: [http, apiKey]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  credential_issuance: manual (contact technical-support@getmymuse.com)\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    in: header\n    header: Authorization\n    value_prefix: 'Bearer '\n    description: >-\n      Short-lived JWT obtained by exchanging\
  \ the issued API key + Client ID +\n      Client Secret at the designated token-exchange endpoint.\n    sources: [docs]\n  - name: apiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: x-api-key\n    description: Static partner API key, issued by Muse Finance support.\n    sources: [docs]\nexample_request: |\n  curl -H \"Authorization: Bearer YOUR_JWT_TOKEN\" \\\n       -H \"x-api-key: YOUR_API_KEY\" \\\n       https://<api-host>/applications\nnotes:\n  - Both headers are required on every request.\n  - No OAuth 2.0 scopes are documented; access is partner-scoped by credential.\n  - The production API base host is not published in the public docs; issued to partners on onboarding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/muse-finance/refs/heads/main/authentication/muse-finance-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Embedded Finance
- Invoice Finance
- Trade Finance
- Lending
- Fintech
- Working Capital
- United Kingdom
---
