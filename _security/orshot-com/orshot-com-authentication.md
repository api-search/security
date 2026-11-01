---
anonymous_access: false
api_key_in: []
auth_types: []
description: Orshot uses OAuth 2.0 for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Orshot Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: orshot-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: orshot-com
provider_slug: orshot-com
scheme_count: 1
schemes:
- authorize_url: https://orshot.com/oauth/authorize
  evidence: 'Register your app : Register it in the dashboard. You get a client_id and client_secret right away.'
  flows:
  - authorization_code
  - device_code
  how_to_obtain: Register an app in the Orshot dashboard to receive a client_id and client_secret.
  name: Orshot OAuth
  type: oauth2
slug: orshot-com-authentication
source_filename: orshot-com-authentication.yml
source_heading: Authentication Profile
source_url: https://orshot.com/docs/developers
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://orshot.com/docs/developers\nsources:\n- https://orshot.com/docs/developers\n- https://orshot.com/docs/developers/examples\n- https://orshot.com/docs/developers/oauth-endpoints\n- https://orshot.com/docs/developers/oauth-overview\ndescription: Orshot uses OAuth 2.0 for authentication.\nschemes:\n- type: oauth2\n  name: Orshot OAuth\n  evidence: 'Register your app : Register it in the dashboard. You get a client_id and client_secret right away.'\n  flows:\n  - authorization_code\n  - device_code\n  authorize_url: https://orshot.com/oauth/authorize\n  how_to_obtain: Register an app in the Orshot dashboard to receive a client_id and client_secret.\nnote: Device Flow token endpoint is https://api.orshot.com/v1/oauth/token and device code endpoint is https://api.orshot.com/v1/oauth/device/code.\ndocs: https://orshot.com/docs/developers\n"
source_yaml_url: https://artifacts.apis.io/orshot-com/authentication/orshot-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API
- Media
- Automation
- AI
---
