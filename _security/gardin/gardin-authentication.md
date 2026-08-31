---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Gardin Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Gardin secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Gardin
provider_slug: gardin
scheme_count: 2
schemes:
- flows:
  - client_auth: HTTP Basic (Base64 of "<CLIENT_ID>:<CLIENT_SECRET>" in Authorization header)
    expires_in_seconds: 3600
    flow: clientCredentials
    grant_type: client_credentials
    scopes_documented: scopes/gardin-scopes.yml
    tokenUrl: https://login.gardin.ag/oauth2/token
    token_format: JWT
    token_type: Bearer
  name: OAuth2ClientCredentials
  sources:
  - docs
  type: oauth2
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - docs
  type: http
  usage: 'Authorization: Bearer {access_token} on all Gardin API requests'
slug: gardin-authentication
source_filename: gardin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.gardin.ag/docs/gardin-api/acquire-access-token-client-credentials-flow\ndocs: https://developers.gardin.ag/docs/gardin-api/gardin-api\nsummary:\n  types: [oauth2, http]\n  oauth2_flows: [clientCredentials]\n  token_format: JWT\n  credentials: Client Id + Client Secret issued by Gardin Support\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.gardin.ag/oauth2/token\n    client_auth: HTTP Basic (Base64 of \"<CLIENT_ID>:<CLIENT_SECRET>\" in Authorization header)\n    grant_type: client_credentials\n    token_type: Bearer\n    token_format: JWT\n    expires_in_seconds: 3600\n    scopes_documented: scopes/gardin-scopes.yml\n  sources: [docs]\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  usage: 'Authorization: Bearer {access_token} on all Gardin API requests'\n  sources: [docs]\nnotes:\n- Client Id and Client\
  \ Secret are provisioned by contacting Gardin Support (no self-service sign-up).\n- The login/token host (login.gardin.ag) does not publish an OIDC/OAuth discovery document (probed 404).\n- Enterprise SSO via Azure AD is documented for portal access at /docs/dev-guide/auth/azuread.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gardin/refs/heads/main/authentication/gardin-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Agriculture
- Agritech
- Precision Agriculture
- Plant Health
- Photosynthesis
- IoT
- Sensors
- Greenhouse
- Crop Intelligence
- Sustainability
- Data
---
