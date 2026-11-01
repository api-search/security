---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Teleship API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Teleship Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teleship declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Teleship
provider_slug: teleship
scheme_count: 1
schemes:
- authorize_url: https://api.teleship.com/oauth/authorize
  evidence: Initiates OAuth 2.0 authorization for partner applications.
  flows:
  - authorization_code
  how_to_obtain: Create an OAuth app in Teleship Shipper Portal to get your clientId and clientSecret.
  name: OAuth 2.0
  scopes:
  - read_accounts
  - write_accounts
  - read_shipments
  - write_shipments
  type: oauth2
slug: teleship-authentication
source_filename: teleship-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.teleship.com/api-reference/authentication/authorize-app.md
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.teleship.com/api-reference/authentication/authorize-app.md\nsources:\n- https://developers.teleship.com/api-reference/authentication/authorize-app.md\n- https://developers.teleship.com/api-reference/authentication/get-access-token.md\n- https://developers.teleship.com/api-reference/authentication/refresh-access-token.md\ndescription: Authentication schemes for Teleship API\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: Initiates OAuth 2.0 authorization for partner applications.\n  flows:\n  - authorization_code\n  authorize_url: https://api.teleship.com/oauth/authorize\n  scopes:\n  - read_accounts\n  - write_accounts\n  - read_shipments\n  - write_shipments\n  how_to_obtain: Create an OAuth app in Teleship Shipper Portal to get your clientId and clientSecret.\ndocs: https://developers.teleship.com/api-reference/authentication/authorize-app.md\n"
source_yaml_url: https://artifacts.apis.io/teleship/authentication/teleship-authentication.yml
summary_line: 1 scheme
tags:
- Shipping
- E‑commerce
- DDP
- Tax
- Integration
- Company
---
