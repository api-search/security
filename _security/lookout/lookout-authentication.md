---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lookout Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Lookout secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Lookout
provider_slug: lookout
scheme_count: 1
schemes:
- base_url: https://api.lookout.com/
  description: The Lookout Mobile Risk API v2 authenticates with the Lookout platform OAuth 2.0 Client Credentials Grant Flow. An administrator generates an application key in the Mobile Endpoint Security (MES) Console; the application exchanges that key for a short-lived bearer access token, which is then sent on each API request. Tokens are scoped to a single Lookout tenant.
  flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - searched:doc.lookout.com
  token_exchange: application key -> access token (bearer)
  type: oauth2
slug: lookout-authentication
source_filename: lookout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://doc.lookout.com/en/mobile-endpoint-security/mes-apis/mobile-risk-api-v2/mobile-risk-api-v2-overview/use-the-mobile-risk-api-version-2\ndocs: https://doc.lookout.com/en/mobile-endpoint-security/mes-apis\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    The Lookout Mobile Risk API v2 authenticates with the Lookout platform OAuth 2.0\n    Client Credentials Grant Flow. An administrator generates an application key in\n    the Mobile Endpoint Security (MES) Console; the application exchanges that key\n    for a short-lived bearer access token, which is then sent on each API request.\n    Tokens are scoped to a single Lookout tenant.\n  token_exchange: application key -> access token (bearer)\n  base_url: https://api.lookout.com/\n  sources:\n  - searched:doc.lookout.com\n\
  notes:\n- The application key is issued and revoked from the MES Console by a tenant administrator.\n- All API endpoints are rate limited to 100 requests per minute per tenant.\n- No fetchable OpenAPI/Swagger definition was retrievable from this environment (the\n  doc portal host doc.lookout.com did not resolve and api.lookout.com returns the\n  console SPA shell), so this profile is documented from the published docs rather\n  than derived from a spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lookout/refs/heads/main/authentication/lookout-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Cybersecurity
- Mobile Security
- Endpoint Security
- Threat Intelligence
- Mobile Threat Defense
- Data Protection
- SIEM
---
