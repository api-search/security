---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hurdlr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hurdlr declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hurdlr
provider_slug: hurdlr
scheme_count: 1
schemes:
- authorize_url: /auth/account
  evidence: 'accessTokenSecurity: type oauth2 flows: implicit: authorizationUrl: /auth/account'
  flows:
  - implicit
  how_to_obtain: Obtain an access token via the OAuth 2.0 implicit flow; the token is returned in the response of the Create a Tight account or Restore a Tight account endpoints.
  name: accessTokenSecurity
  scopes:
  - write
  type: oauth2
slug: hurdlr-authentication
source_filename: hurdlr-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.tight.com/v4.0/api-reference/authentication/create-a-tight-account.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.tight.com/v4.0/api-reference/authentication/create-a-tight-account.md\nsources:\n- https://docs.tight.com/v4.0/api-reference/authentication/create-a-tight-account.md\n- https://docs.tight.com/v4.0/api-reference/authentication/delete-a-tight-account.md\n- https://docs.tight.com/v4.0/api-reference/authentication/restore-a-tight-account.md\n- https://docs.tight.com/v4.0/api-reference/authentication/refresh-access-token.md\ndescription: Authentication\nschemes:\n- type: oauth2\n  name: accessTokenSecurity\n  evidence: 'accessTokenSecurity: type oauth2 flows: implicit: authorizationUrl: /auth/account'\n  flows:\n  - implicit\n  authorize_url: /auth/account\n  scopes:\n  - write\n  how_to_obtain: Obtain an access token via the OAuth 2.0 implicit flow; the token is returned in the response of the Create a Tight account or\n    Restore a Tight account endpoints.\ndocs: https://docs.tight.com/v4.0/api-reference/authentication/create-a-tight-account.md\n"
source_yaml_url: https://artifacts.apis.io/hurdlr/authentication/hurdlr-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Finance
- Expense Tracking
- Mileage Tracking
- Tax Automation
- Invoicing
---
