---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Brightflag Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Brightflag secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Brightflag
provider_slug: brightflag
scheme_count: 2
schemes:
- flow: clientCredentials
  name: OAuth2
  region_specific_base_url: true
  source: docs
  token_endpoint: '{BASE_URL}/oauth/token'
  token_response: access_token, token_type=bearer, expires_in, scope
  type: oauth2
- bearer_format: JWT/opaque access token from the OAuth token endpoint
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  source: docs
  type: http
slug: brightflag-authentication
source_filename: brightflag-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://help.brightflag.com/hc/en-us/articles/26006518363293-How-to-Get-an-API-Token-for-Brightflag\ndocs: https://help.brightflag.com/hc/en-us/categories/21136642887581-API\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  notes: Brightflag's API uses OAuth 2.0. Clients POST to {BASE_URL}/oauth/token to\n    exchange credentials for a bearer access_token, then send that token in the HTTP\n    Authorization header on every request. The token response returns access_token,\n    token_type \"bearer\", an expiry, and a scope. API credentials are generated inside\n    the product admin area (Admin > API access) at the developer portal.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: clientCredentials\n  token_endpoint: '{BASE_URL}/oauth/token'\n  token_response: access_token, token_type=bearer, expires_in, scope\n  region_specific_base_url: true\n  source: docs\n- name: bearerAuth\n\
  \  type: http\n  scheme: bearer\n  bearer_format: JWT/opaque access token from the OAuth token endpoint\n  in: header\n  header: Authorization\n  source: docs\ncredential_provisioning:\n  where: Admin > API access in the Brightflag app\n  portal: https://app.brightflag.com/developer\n  note: API tokens are self-service for admins; API-based reporting setup may require\n    contacting your Customer Success Manager.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightflag/refs/heads/main/authentication/brightflag-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Legal
- Legal Operations
- Legal Spend Management
- Enterprise Legal Management
- E-Billing
- Matter Management
- Reporting
- Artificial Intelligence
- LegalTech
---
