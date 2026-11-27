---
anonymous_access: false
api_key_in: []
auth_types: []
description: Scout uses OAuth2 authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Scout Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scout declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Scout
provider_slug: dinewithscout-com
scheme_count: 1
schemes:
- authorize_url: https://dinewithscout.com/oauth/authorize
  evidence: '"authorization_endpoint":"https://dinewithscout.com/oauth/authorize"'
  flows:
  - authorization_code
  name: Scout OAuth2
  scopes:
  - requests:read
  - requests:write
  - reservations:read
  - restaurants:read
  type: oauth2
slug: dinewithscout-com-authentication
source_filename: dinewithscout-com-authentication.yml
source_heading: Authentication Profile
source_url: https://dinewithscout.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dinewithscout.com/.well-known/oauth-authorization-server\nsources:\n- https://dinewithscout.com/.well-known/oauth-authorization-server\n- https://dinewithscout.com/.well-known/oauth-protected-resource/mcp\ndescription: Scout uses OAuth2 authentication.\nschemes:\n- type: oauth2\n  name: Scout OAuth2\n  evidence: '\"authorization_endpoint\":\"https://dinewithscout.com/oauth/authorize\"'\n  flows:\n  - authorization_code\n  authorize_url: https://dinewithscout.com/oauth/authorize\n  scopes:\n  - requests:read\n  - requests:write\n  - reservations:read\n  - restaurants:read\ndocs: https://dinewithscout.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/dinewithscout-com/authentication/dinewithscout-com-authentication.yml
summary_line: 1 scheme
tags:
- Restaurant
- Reservations
- Automation
- Software-as-a-Service
- Consumer
---
