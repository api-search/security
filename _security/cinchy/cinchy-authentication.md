---
api_key_in: []
auth_types:
- http
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cinchy Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cinchy secures its APIs with http, oauth2, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cinchy
provider_slug: cinchy
scheme_count: 4
schemes:
- description: Access token obtained from the OAuth2 token endpoint (/identity/connect/token), passed in the Authorization header.
  name: bearerToken
  scheme: bearer
  type: http
- description: User-generated Personal Access Token (PAT) passed as a bearer token in the Authorization header for API access.
  name: personalAccessToken
  scheme: bearer
  type: http
- description: HTTP Basic authentication via the /BasicAuthAPI/ URL prefix as an alternative to bearer tokens.
  name: basicAuth
  scheme: basic
  type: http
- description: OAuth2-style token endpoint (IdentityServer) used to obtain access tokens for programmatic API access.
  flow: clientCredentials
  name: oauth2ClientCredentials
  tokenUrl: <baseurl>/identity/connect/token
  type: oauth2
slug: cinchy-authentication
source_filename: cinchy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.cinchy.com/api-guide/\ndocs: https://docs.cinchy.com/api-guide/\nsummary:\n  types: [http, oauth2, apiKey]\n  http_schemes: [bearer, basic]\n  oauth2_flows: [clientCredentials]\n  notes: >-\n    Cinchy is a per-tenant deployed platform (self-hosted or Cinchy-hosted), so\n    the base URL is tenant-specific. Authentication is served by an embedded\n    IdentityServer (OAuth2/OIDC) at the /identity/connect/token endpoint.\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    description: >-\n      Access token obtained from the OAuth2 token endpoint (/identity/connect/token),\n      passed in the Authorization header.\n  - name: personalAccessToken\n    type: http\n    scheme: bearer\n    description: >-\n      User-generated Personal Access Token (PAT) passed as a bearer token in the\n      Authorization header for API access.\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description:\
  \ >-\n      HTTP Basic authentication via the /BasicAuthAPI/ URL prefix as an alternative\n      to bearer tokens.\n  - name: oauth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: \"<baseurl>/identity/connect/token\"\n    description: >-\n      OAuth2-style token endpoint (IdentityServer) used to obtain access tokens for\n      programmatic API access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cinchy/refs/heads/main/authentication/cinchy-authentication.yml
summary_line: http/oauth2/apiKey · 4 schemes
tags:
- Company
- Data
- Data Collaboration
- Dataware
- Data Integration
- Data Governance
- AI Governance
- API
---
