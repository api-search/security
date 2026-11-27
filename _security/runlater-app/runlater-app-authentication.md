---
anonymous_access: false
api_key_in: []
api_specs:
- filename: runlater-app-account-api-openapi.yml
  format: yaml
  label: RunLater Account API
  slug: runlater-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/runlater-app/openapi/runlater-app-account-api-openapi.yml
- filename: runlater-app-runs-api-openapi.yml
  format: yaml
  label: RunLater Runs API
  slug: runlater-app-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/runlater-app/openapi/runlater-app-runs-api-openapi.yml
- filename: runlater-app-schedules-api-openapi.yml
  format: yaml
  label: RunLater Schedules API
  slug: runlater-app-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/runlater-app/openapi/runlater-app-schedules-api-openapi.yml
auth_types: []
description: Authentication methods for RunLater API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: RunLater Authentication
name_suffix: Authentication
oauth_flows: []
overview: RunLater declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: RunLater
provider_slug: runlater-app
scheme_count: 3
schemes:
- evidence: 'Authorization: Bearer rl_sk_...'
  header: Authorization
  how_to_obtain: Create a key in Settings under API keys; the key starts with rl_sk_ and is shown once.
  location: header
  name: Bearer
  type: http-bearer
- evidence: 'X-API-Key: your-api-key-here'
  header: X-API-Key
  how_to_obtain: Create a key in Settings under API keys; the key starts with rl_sk_ and is shown once.
  location: header
  name: API Key
  type: apiKey
- evidence: 'Authorization: Basic dXNlcm5hbWU6cGFzc3dvcmQ='
  header: Authorization
  how_to_obtain: Provide a username and password; the value is base64(username:password).
  location: header
  name: Basic Auth
  type: http-basic
slug: runlater-app-authentication
source_filename: runlater-app-authentication.yml
source_heading: Authentication Profile
source_url: https://runlater.app/docs/api
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://runlater.app/docs/api\nsources:\n- https://runlater.app/docs/api\n- https://runlater.app/docs/guides/headers-and-auth\n- https://runlater.app/auth.md\n- https://runlater.app/docs/guides/request-signing\ndescription: Authentication methods for RunLater API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization: Bearer rl_sk_...'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Settings under API keys; the key starts with rl_sk_ and is shown once.\n- type: apiKey\n  name: API Key\n  evidence: 'X-API-Key: your-api-key-here'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a key in Settings under API keys; the key starts with rl_sk_ and is shown once.\n- type: http-basic\n  name: Basic Auth\n  evidence: 'Authorization: Basic dXNlcm5hbWU6cGFzc3dvcmQ='\n  location: header\n  header: Authorization\n  how_to_obtain:\
  \ Provide a username and password; the value is base64(username:password).\nnote: OAuth flows are not described for RunLater; only bearer token, API key, and basic auth are documented.\ndocs: https://runlater.app/docs/api\n"
source_yaml_url: https://artifacts.apis.io/runlater-app/authentication/runlater-app-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Scheduler
- Webhook
- Automation
---
