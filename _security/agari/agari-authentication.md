---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Agari Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Agari secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Agari
provider_slug: agari
scheme_count: 1
schemes:
- credential_provisioning: manual (generated in the Agari product portal)
  flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - https://developers.agari.com/agari-platform/docs/oauth-20
  token_lifetime_seconds: 14400
  token_presentation: bearer access_token on API requests
  token_url: https://api.agari.com/v1/ep/token
  type: oauth2
slug: agari-authentication
source_filename: agari-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developers.agari.com/agari-platform/docs/oauth-20\ndocs: https://developers.agari.com/agari-platform/docs/access-and-authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_lifetime: 4 hours\n  notes: >-\n    The Agari Platform APIs use OAuth 2.0 with the Client Credentials grant.\n    A client_id and client_secret are generated manually in the product portal,\n    then exchanged at the token endpoint for a temporary bearer access_token\n    valid for four hours. The access_token is presented on subsequent API\n    requests. There is no documented per-scope authorization surface.\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://api.agari.com/v1/ep/token\n    token_lifetime_seconds: 14400\n    credential_provisioning: manual (generated in the Agari product portal)\n    token_presentation: bearer access_token on API requests\n\
  \    sources: [https://developers.agari.com/agari-platform/docs/oauth-20]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agari/refs/heads/main/authentication/agari-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Email Security
- Cybersecurity
- DMARC
- Email Authentication
- Phishing
- Anti-Phishing
- Brand Protection
- API
- REST
---
