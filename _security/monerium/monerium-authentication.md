---
anonymous_access: false
api_key_in: []
api_specs:
- filename: monerium-openapi.yml
  format: yaml
  label: Monerium API
  slug: monerium-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monerium/openapi/monerium-openapi.yml
auth_types: []
description: Monerium uses OAuth 2.0 Authorization Code flow with PKCE for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Monerium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Monerium declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Monerium
provider_slug: monerium
scheme_count: 1
schemes:
- authorize_url: https://api.monerium.dev/auth
  evidence: The OAuth flow uses Authorization Code with PKCE .
  flows:
  - authorization_code
  how_to_obtain: Create an application in the Monerium sandbox or production portal and copy the CLIENT ID from the credentials screen.
  name: OAuth 2.0
  type: oauth2
slug: monerium-authentication
source_filename: monerium-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.monerium.com/oauth/
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.monerium.com/oauth/\nsources:\n- https://docs.monerium.com/oauth/\n- https://docs.monerium.com/packages/sdk/interfaces/Token/\n- https://docs.monerium.com/token-integration/\n- https://docs.monerium.com/tokens/\ndescription: Monerium uses OAuth 2.0 Authorization Code flow with PKCE for authentication.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: The OAuth flow uses Authorization Code with PKCE .\n  flows:\n  - authorization_code\n  authorize_url: https://api.monerium.dev/auth\n  how_to_obtain: Create an application in the Monerium sandbox or production portal and copy the CLIENT ID from the credentials screen.\nnote: Token endpoint is https://api.monerium.dev/auth/token as shown in the token exchange examples.\ndocs: https://docs.monerium.com/oauth/\n"
source_yaml_url: https://artifacts.apis.io/monerium/authentication/monerium-authentication.yml
summary_line: 1 scheme
tags:
- FinTech
- Payments
- Blockchain
- DigitalCurrency
- RegulatedMoney
---
