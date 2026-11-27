---
anonymous_access: false
api_key_in: []
api_specs:
- filename: avnester-com-public-api-openapi.yml
  format: yaml
  label: AVnester Public API
  slug: avnester-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avnester-com/openapi/avnester-com-public-api-openapi.yml
auth_types: []
description: Authentication methods for AVnester APIs
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: AVnester Authentication
name_suffix: Authentication
oauth_flows: []
overview: AVnester declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: AVnester
provider_slug: avnester-com
scheme_count: 3
schemes:
- authorize_url: https://auth.avnester.com/oauth/authorize
  evidence: Redirect the user to https://auth.avnester.com/oauth/authorize ?response_type=code&client_id=...&redirect_uri=...&code_challenge=...&code_challenge_method=S256&scope= calculators:use%20listings:read:public%20locality:read:public
  flows:
  - authorization_code
  how_to_obtain: Register a client via Dynamic Client Registration (DCR) to obtain a client_id, then run the PKCE flow.
  name: Authorization Code with PKCE
  scopes:
  - calculators:use
  - listings:read:public
  - locality:read:public
  type: oauth2
- evidence: 'POST https://auth.avnester.com/oauth/token , form-encoded: grant_type=client_credentials scope : one or more of the credential’s scopes, space-separated.'
  flows:
  - client_credentials
  how_to_obtain: Create an OAuth client credential (signed key or client secret) in the developer console, then exchange it at the token endpoint.
  name: Client Credentials
  token_url: https://auth.avnester.com/oauth/token
  type: oauth2
- evidence: Send it in the Authorization header with the Bearer scheme, on every request.
  header: Authorization
  how_to_obtain: Create an API key in the developer console under Server credentials.
  location: header
  name: API Key
  type: http-bearer
slug: avnester-com-authentication
source_filename: avnester-com-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.avnester.com/oauth
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.avnester.com/oauth\nsources:\n- https://developers.avnester.com/oauth\n- https://developers.avnester.com/server-credentials\ndescription: Authentication methods for AVnester APIs\nschemes:\n- type: oauth2\n  name: Authorization Code with PKCE\n  evidence: Redirect the user to https://auth.avnester.com/oauth/authorize ?response_type=code&client_id=...&redirect_uri=...&code_challenge=...&code_challenge_method=S256&scope=\n    calculators:use%20listings:read:public%20locality:read:public\n  flows:\n  - authorization_code\n  authorize_url: https://auth.avnester.com/oauth/authorize\n  scopes:\n  - calculators:use\n  - listings:read:public\n  - locality:read:public\n  how_to_obtain: Register a client via Dynamic Client Registration (DCR) to obtain a client_id, then run the PKCE flow.\n- type: oauth2\n  name: Client Credentials\n  evidence: 'POST https://auth.avnester.com/oauth/token\
  \ , form-encoded: grant_type=client_credentials scope : one or more of the credential’s\n    scopes, space-separated.'\n  flows:\n  - client_credentials\n  token_url: https://auth.avnester.com/oauth/token\n  how_to_obtain: Create an OAuth client credential (signed key or client secret) in the developer console, then exchange it at the token endpoint.\n- type: http-bearer\n  name: API Key\n  evidence: Send it in the Authorization header with the Bearer scheme, on every request.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the developer console under Server credentials.\ndocs: https://developers.avnester.com/oauth\n"
source_yaml_url: https://artifacts.apis.io/avnester-com/authentication/avnester-com-authentication.yml
summary_line: 3 schemes
tags:
- Real Estate
- Artificial Intelligence
- Property Listings
- India
- Marketplace
---
