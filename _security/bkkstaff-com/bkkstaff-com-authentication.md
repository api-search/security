---
anonymous_access: false
api_key_in: []
auth_types: []
description: OAuth2 authorization code flow
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: BKK Staff Authentication
name_suffix: Authentication
oauth_flows: []
overview: BKK Staff declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BKK Staff
provider_slug: bkkstaff-com
scheme_count: 1
schemes:
- authorize_url: https://app.bkkstaff.com/oauth/authorize
  evidence: '"authorization_endpoint":"https://app.bkkstaff.com/oauth/authorize"'
  flows:
  - authorization_code
  how_to_obtain: via the OAuth 2.0 authorization endpoint
  name: OAuth2
  scopes:
  - mcp
  type: oauth2
slug: bkkstaff-com-authentication
source_filename: bkkstaff-com-authentication.yml
source_heading: Authentication Profile
source_url: https://app.bkkstaff.com/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://app.bkkstaff.com/.well-known/oauth-protected-resource\nsources:\n- https://app.bkkstaff.com/.well-known/oauth-protected-resource\n- https://app.bkkstaff.com/.well-known/oauth-authorization-server\ndescription: OAuth2 authorization code flow\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: '\"authorization_endpoint\":\"https://app.bkkstaff.com/oauth/authorize\"'\n  flows:\n  - authorization_code\n  authorize_url: https://app.bkkstaff.com/oauth/authorize\n  scopes:\n  - mcp\n  how_to_obtain: via the OAuth 2.0 authorization endpoint\ndocs: https://app.bkkstaff.com/.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/bkkstaff-com/authentication/bkkstaff-com-authentication.yml
summary_line: 1 scheme
tags:
- Hiring
- Staffing
- Small Business
- Automation
- Thailand
---
