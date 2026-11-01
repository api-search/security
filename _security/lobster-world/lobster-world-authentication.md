---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lobster-world-channels-api-openapi.yml
  format: yaml
  label: Lobster Data GmbH Channels API
  slug: lobster-world-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lobster-world/openapi/lobster-world-channels-api-openapi.yml
auth_types: []
description: OAuth2 authentication for HTTP channels
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lobster World Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lobster Data GmbH declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lobster Data GmbH
provider_slug: lobster-world
scheme_count: 1
schemes:
- evidence: Da im Dialog sowohl der Authorization Header als auch der Wert angepasst werden kann, kann die Option ebenso für API Keys oder andere Autorisierungsarten, bei denen ein Header benötigt wird, verwendet werden!
  flows:
  - authorization_code
  - client_credentials
  - password
  how_to_obtain: Enter Client ID, Client Secret and other required credentials in the channel configuration wizard (OAuth2.0 konfigurieren).
  name: OAuth2
  token_url: https://<server>/oauth/token
  type: oauth2
slug: lobster-world-authentication
source_filename: lobster-world-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.lobstersoftware.com/docs/tutorials-oauth-2.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.lobstersoftware.com/docs/tutorials-oauth-2.md\nsources:\n- https://docs.lobstersoftware.com/docs/tutorials-oauth-2.md\n- https://docs.lobstersoftware.com/docs/basic-change-oauth-2-access-token.md\n- https://docs.lobstersoftware.com/docs/core-authentication-event.md\n- https://docs.lobstersoftware.com/docs/core-authentication-event-registered-login.md\ndescription: OAuth2 authentication for HTTP channels\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: Da im Dialog sowohl der Authorization Header als auch der Wert angepasst werden kann, kann die Option ebenso für API Keys oder andere\n    Autorisierungsarten, bei denen ein Header benötigt wird, verwendet werden!\n  flows:\n  - authorization_code\n  - client_credentials\n  - password\n  token_url: https://<server>/oauth/token\n  how_to_obtain: Enter Client ID, Client Secret and other required credentials in the\
  \ channel configuration wizard (OAuth2.0 konfigurieren).\ndocs: https://docs.lobstersoftware.com/docs/tutorials-oauth-2.md\n"
source_yaml_url: https://artifacts.apis.io/lobster-world/authentication/lobster-world-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data
- Analytics
- IoT
- Real-Time
---
