---
anonymous_access: false
api_key_in: []
api_specs:
- filename: par-technology-auth-api-openapi.yml
  format: yaml
  label: PAR Technology Auth API
  slug: par-technology-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/par-technology/refs/heads/main/openapi/par-technology-auth-api-openapi.yml
- filename: par-technology-discounts-api-openapi.yml
  format: yaml
  label: PAR Technology Discounts API
  slug: par-technology-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/par-technology/refs/heads/main/openapi/par-technology-discounts-api-openapi.yml
- filename: par-technology-pos-api-openapi.yml
  format: yaml
  label: PAR Technology Pos API
  slug: par-technology-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/par-technology/refs/heads/main/openapi/par-technology-pos-api-openapi.yml
- filename: par-technology-redemptions-api-openapi.yml
  format: yaml
  label: PAR Technology Redemptions API
  slug: par-technology-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/par-technology/refs/heads/main/openapi/par-technology-redemptions-api-openapi.yml
auth_types: []
description: Authentication methods published by PAR Technology
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Par Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: PAR Technology declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: PAR Technology
provider_slug: par-technology
scheme_count: 2
schemes:
- evidence: Retrieves a client instance-level access token from your redirect URI after a successful user login through the Punchh-hosted authentication form.
  how_to_obtain: Provide client_id, client_secret, authorization code, redirect_uri, and grant_type=authorization_code in a POST request to the token endpoint as shown in the request example.
  name: OAuth 2.0
  token_url: https://SERVER_NAME_GOES_HERE.punchh.com/oauth/token
  type: oauth2
- evidence: Get your API key - Use a valid OAuth client key from the Punchh platform to send requests to the API endpoints.
  how_to_obtain: Obtain the OAuth client key from the Punchh platform (provided by your PAR Punchh representative).
  name: API Key (OAuth client key)
  type: other
slug: par-technology-authentication
source_filename: par-technology-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.partech.com/docs/dev-portal-developer-resources/developer-guides/advanced-auth-developer-guide
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.partech.com/docs/dev-portal-developer-resources/developer-guides/advanced-auth-developer-guide\nsources:\n- https://developers.partech.com/docs/dev-portal-developer-resources/developer-guides/advanced-auth-developer-guide\n- https://developers.partech.com/docs/dev-portal-mobile/additional-topics/user-authentication\n- https://developers.partech.com/docs/dev-portal-online-ordering/apis/online-ordering-and-sso-api/tag/user-sign-up-and-sso/post/oauth/token\n- https://developers.partech.com/docs/identity-service/advanced-authentication\ndescription: Authentication methods published by PAR Technology\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: Retrieves a client instance-level access token from your redirect URI after a successful user login through the Punchh-hosted authentication\n    form.\n  token_url: https://SERVER_NAME_GOES_HERE.punchh.com/oauth/token\n\
  \  how_to_obtain: Provide client_id, client_secret, authorization code, redirect_uri, and grant_type=authorization_code in a POST request to the\n    token endpoint as shown in the request example.\n- type: other\n  name: API Key (OAuth client key)\n  evidence: Get your API key - Use a valid OAuth client key from the Punchh platform to send requests to the API endpoints.\n  how_to_obtain: Obtain the OAuth client key from the Punchh platform (provided by your PAR Punchh representative).\ndocs: https://developers.partech.com/docs/dev-portal-developer-resources/developer-guides/advanced-auth-developer-guide\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/par-technology/refs/heads/main/authentication/par-technology-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Hospitality
- Point-of-Sale
- Loyalty
- Retail
---
