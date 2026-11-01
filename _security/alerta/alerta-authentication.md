---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods documented for Alerta
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Alerta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alerta declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Alerta
provider_slug: alerta
scheme_count: 4
schemes:
- evidence: The most straight-forward authentication strategy to implement of the four is HTTP Basic Authentication provided by the Alerta API because there is no additional configuration required of the Alerta server to use it other than setting AUTH_REQUIRED to True .
  header: Authorization
  how_to_obtain: Users sign up via the web UI or using the CLI and then login to receive a JWT token.
  location: header
  name: Basic Auth
  type: http-basic
- evidence: The API Keys page allows you to create and manage API keys used to authenticate with the Alerta API.
  how_to_obtain: Create a new API key via the Alerta UI (Configuration > API Keys) or through the API.
  name: API Keys
  type: apiKey
- evidence: To use GitHub as the OAuth2 provider for Alerta, login to GitHub and go to Settings -> Applications -> Register New Application .
  how_to_obtain: Register an application in GitHub and configure Alerta to use it.
  name: GitHub OAuth2
  type: oauth2
- evidence: 'Alerta also supports two “machine-to-machine” authentication strategies: API Keys, HMAC Auth'
  name: HMAC Auth
  type: other
slug: alerta-authentication
source_filename: alerta-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.alerta.io/webui/apikeys.html
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.alerta.io/webui/apikeys.html\nsources:\n- https://docs.alerta.io/webui/apikeys.html\n- https://docs.alerta.io/authentication.html\n- https://docs.alerta.io/gettingstarted/tutorial-6-auth.html\n- https://docs.alerta.io/webui/authentication.html\ndescription: Authentication methods documented for Alerta\nschemes:\n- type: http-basic\n  name: Basic Auth\n  evidence: The most straight-forward authentication strategy to implement of the four is HTTP Basic Authentication provided by the Alerta API\n    because there is no additional configuration required of the Alerta server to use it other than setting AUTH_REQUIRED to True .\n  location: header\n  header: Authorization\n  how_to_obtain: Users sign up via the web UI or using the CLI and then login to receive a JWT token.\n- type: apiKey\n  name: API Keys\n  evidence: The API Keys page allows you to create and manage API\
  \ keys used to authenticate with the Alerta API.\n  how_to_obtain: Create a new API key via the Alerta UI (Configuration > API Keys) or through the API.\n- type: oauth2\n  name: GitHub OAuth2\n  evidence: To use GitHub as the OAuth2 provider for Alerta, login to GitHub and go to Settings -> Applications -> Register New Application .\n  how_to_obtain: Register an application in GitHub and configure Alerta to use it.\n- type: other\n  name: HMAC Auth\n  evidence: 'Alerta also supports two “machine-to-machine” authentication strategies: API Keys, HMAC Auth'\ndocs: https://docs.alerta.io/webui/apikeys.html\n"
source_yaml_url: https://artifacts.apis.io/alerta/authentication/alerta-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Alerting
- Monitoring
- OpenSource
- DevOps
- IncidentManagement
---
