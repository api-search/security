---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cloudcheckr-openapi-generated.yml
  format: yaml
  label: CloudCheckr API
  slug: cloudcheckr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudcheckr/refs/heads/main/openapi/_ae-authored/cloudcheckr-openapi-generated.yml
auth_types: []
description: Flexera One API authentication uses OAuth2 access tokens.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cloudcheckr Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudCheckr declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CloudCheckr
provider_slug: cloudcheckr
scheme_count: 1
schemes:
- evidence: Authenticated requests include an API Access Token which proves the caller's identity.
  how_to_obtain: Create a refresh token via the Flexera One UI (API Credentials) for user authentication, or obtain a clientId and clientSecret for a service account. Then POST to the token URL with grant_type=refresh_token&refresh_token=<refresh token> (user) or grant_type=client_credentials&client_id=<client Id>&client_secret=<client secret> (service account).
  name: Flexera One OAuth2
  token_url: https://login.flexera.com/oidc/token
  type: oauth2
slug: cloudcheckr-authentication
source_filename: cloudcheckr-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.flexera.com/docs/page/authentication
source_yaml: "generated: '2026-10-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.flexera.com/docs/page/authentication\nsources:\n- https://developer.flexera.com/docs/page/authentication\ndescription: Flexera One API authentication uses OAuth2 access tokens.\nschemes:\n- type: oauth2\n  name: Flexera One OAuth2\n  evidence: Authenticated requests include an API Access Token which proves the caller's identity.\n  token_url: https://login.flexera.com/oidc/token\n  how_to_obtain: Create a refresh token via the Flexera One UI (API Credentials) for user authentication, or obtain a clientId and clientSecret\n    for a service account. Then POST to the token URL with grant_type=refresh_token&refresh_token=<refresh token> (user) or grant_type=client_credentials&client_id=<client\n    Id>&client_secret=<client secret> (service account).\nnote: Access tokens must be sent in the Authorization header as \"Bearer <access token>\".\ndocs: https://developer.flexera.com/docs/page/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudcheckr/refs/heads/main/authentication/cloudcheckr-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Cloud Cost Management
- FinOps
- MSP
- Enterprise
- Flexera
---
