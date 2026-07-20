---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Agari Data Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Agari Data secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Agari Data
provider_slug: agari-data
scheme_count: 1
schemes:
- bearer_header: 'Authorization: Bearer <access_token>'
  flow: clientCredentials
  name: OAuth2ClientCredentials
  regional_token_urls:
  - product: Cloud Email Protection (US)
    url: https://api.agari.com/v1/ep/token
  - product: Brand Protection (US)
    url: https://api.agari.com/v1/cp/token
  - product: Brand Protection (EU)
    url: https://api.agari-eu.com/v1/cp/token
  sources:
  - https://developers.agari.com/agari-platform/docs/oauth-20
  token_lifetime_seconds: 14400
  token_url: https://api.agari.com/v1/ep/token
  type: oauth2
slug: agari-data-authentication
source_filename: agari-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developers.agari.com/agari-platform/docs/oauth-20\ndocs: https://developers.agari.com/agari-platform/docs/access-and-authentication\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    The Agari Platform API uses OAuth 2.0 with the client-credentials grant. A client_id and\n    client_secret are generated in the Agari platform, then exchanged at the token endpoint for a\n    temporary bearer access_token that is sent on every API request as an Authorization: Bearer\n    header. Access tokens are valid for 4 hours (14400 seconds); after expiry a new token must be\n    requested. No user-scoped OAuth (authorization code) flow and no API-key mechanism are documented.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.agari.com/v1/ep/token\n  token_lifetime_seconds: 14400\n  bearer_header: 'Authorization: Bearer <access_token>'\n\
  \  regional_token_urls:\n  - product: Cloud Email Protection (US)\n    url: https://api.agari.com/v1/ep/token\n  - product: Brand Protection (US)\n    url: https://api.agari.com/v1/cp/token\n  - product: Brand Protection (EU)\n    url: https://api.agari-eu.com/v1/cp/token\n  sources:\n  - https://developers.agari.com/agari-platform/docs/oauth-20\nscopes: []\nscopes_note: The docs do not publish a named OAuth scope/permission reference; access is per client credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agari-data/refs/heads/main/authentication/agari-data-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Email Security
- Phishing Protection
- DMARC
- Business Email Compromise
- Threat Intelligence
- Cybersecurity
---
