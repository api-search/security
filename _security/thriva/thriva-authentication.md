---
api_key_in: []
api_specs:
- filename: thriva-appointments-api-api-openapi.yml
  format: yaml
  label: Thriva Appointments API API
  slug: thriva-appointments-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-appointments-api-api-openapi.yml
- filename: thriva-auth-api-api-openapi.yml
  format: yaml
  label: Thriva Auth API API
  slug: thriva-auth-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-auth-api-api-openapi.yml
- filename: thriva-biomarkers-api-api-openapi.yml
  format: yaml
  label: Thriva Biomarkers API API
  slug: thriva-biomarkers-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-biomarkers-api-api-openapi.yml
- filename: thriva-bulk-orders-api-api-openapi.yml
  format: yaml
  label: Thriva Bulk Orders API API
  slug: thriva-bulk-orders-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-bulk-orders-api-api-openapi.yml
- filename: thriva-escalations-api-api-openapi.yml
  format: yaml
  label: Thriva Escalations API API
  slug: thriva-escalations-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-escalations-api-api-openapi.yml
- filename: thriva-orders-api-api-openapi.yml
  format: yaml
  label: Thriva Orders API API
  slug: thriva-orders-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-orders-api-api-openapi.yml
- filename: thriva-result-attachments-api-api-openapi.yml
  format: yaml
  label: Thriva Result attachments API API
  slug: thriva-result-attachments-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-result-attachments-api-api-openapi.yml
- filename: thriva-results-api-api-openapi.yml
  format: yaml
  label: Thriva Results API API
  slug: thriva-results-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-results-api-api-openapi.yml
- filename: thriva-tracking-api-api-openapi.yml
  format: yaml
  label: Thriva Tracking API API
  slug: thriva-tracking-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-tracking-api-api-openapi.yml
- filename: thriva-users-api-api-openapi.yml
  format: yaml
  label: Thriva Users API API
  slug: thriva-users-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/openapi/thriva-users-api-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Thriva Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Thriva secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Thriva
provider_slug: thriva
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    notes: The token request must include an `audience` parameter; for sandbox use, the audience is the Sandbox API URL (https://api.euw2.sandbox.thriva.io/). The Platform API reference also documents the token operation as POST /oauth/token ("Create OAuth Token").
    sandbox_tokenUrl: https://auth.sandbox.thriva.io/oauth/token
    tokenUrl: https://auth.thriva.io/oauth/token
  name: OAuth2ClientCredentials
  sources:
  - https://docs.thriva.io/docs/authentication
  - https://docs.thriva.io/reference/post_oauth-token
  - well-known/thriva-openid-configuration.json
  type: oauth2
slug: thriva-authentication
source_filename: thriva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://docs.thriva.io/docs/authentication\nsource: https://docs.thriva.io/docs/authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_style: bearer\noverview: >-\n  Access to the Thriva Platform API is enforced through the OAuth 2.0 Client Credentials\n  grant. Thriva provisions each partner with a clientId and secret, which are exchanged for\n  an access token at the Auth API; the access token is then used as a bearer token on\n  Platform API requests. The Auth API is Auth0-backed: both production and sandbox auth\n  hosts publish OIDC discovery documents (captured in well-known/).\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://auth.thriva.io/oauth/token\n        sandbox_tokenUrl: https://auth.sandbox.thriva.io/oauth/token\n        notes: >-\n          The token request must include an `audience` parameter;\
  \ for sandbox use, the\n          audience is the Sandbox API URL (https://api.euw2.sandbox.thriva.io/). The\n          Platform API reference also documents the token operation as POST /oauth/token\n          (\"Create OAuth Token\").\n    sources:\n      - https://docs.thriva.io/docs/authentication\n      - https://docs.thriva.io/reference/post_oauth-token\n      - well-known/thriva-openid-configuration.json\ndiscovery:\n  production_oidc: https://auth.thriva.io/.well-known/openid-configuration\n  sandbox_oidc: https://auth.sandbox.thriva.io/.well-known/openid-configuration\n  jwks: https://auth.thriva.io/.well-known/jwks.json\nnotes: >-\n  The published OpenAPI declares no securitySchemes; this profile is taken from the\n  provider's authentication documentation and the live OIDC discovery documents. No\n  partner-facing OAuth scopes are documented for the Platform API (the client-credentials\n  grant is unscoped in the docs), so no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thriva/refs/heads/main/authentication/thriva-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Healthcare
- Diagnostics
- Blood Testing
- At-Home Testing
- Digital Health
- Lab Testing
- Webhooks
- United Kingdom
---
