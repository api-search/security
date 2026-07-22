---
api_key_in:
- header
auth_types:
- http-basic
- publishable-key
- launch-token
description: ''
kind: authentication
layout: security
method: searched
name: Tortus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tortus secures its APIs with http-basic, publishable-key, and launch-token across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tortus
provider_slug: tortus
scheme_count: 3
schemes:
- description: 'Your backend authenticates to the TORTUS launch endpoint with HTTP Basic Authentication: username = client ID (e.g. cli_abc123xyz), password = client secret (e.g. sec_def456uvw), base64-encoded as clientId:clientSecret in the Authorization header. Never expose the client ID/secret to the frontend.'
  location: POST https://api.tortus.ai/v1/oauth/launch (server-side only)
  name: launchEndpointBasicAuth
  scheme: basic
  type: http
- description: Public identifier (pk_...) passed to loadTortus() in the browser to identify the tenant. Safe to expose to the frontend.
  in: config
  name: publishableKey
  parameter: publishableKey
  type: apiKey
- description: Short-lived launch token minted by the launch endpoint and returned to the SDK via the fetchClientSecrets() callback. The SDK exchanges it to load and authenticate the embedded app. Tokens expire after 5 minutes and must be requested fresh per session.
  name: launchToken
  scheme: bearer
  type: http
slug: tortus-authentication
source_filename: tortus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tortus.ai/authentication\ndocs: https://docs.tortus.ai/authentication\nsummary:\n  types: [http-basic, publishable-key, launch-token]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: launchEndpointBasicAuth\n    type: http\n    scheme: basic\n    location: \"POST https://api.tortus.ai/v1/oauth/launch (server-side only)\"\n    description: >-\n      Your backend authenticates to the TORTUS launch endpoint with HTTP Basic\n      Authentication: username = client ID (e.g. cli_abc123xyz), password =\n      client secret (e.g. sec_def456uvw), base64-encoded as clientId:clientSecret\n      in the Authorization header. Never expose the client ID/secret to the\n      frontend.\n  - name: publishableKey\n    type: apiKey\n    in: config\n    parameter: publishableKey\n    description: >-\n      Public identifier (pk_...) passed to loadTortus() in the browser to\n      identify the tenant. Safe to expose\
  \ to the frontend.\n  - name: launchToken\n    type: http\n    scheme: bearer\n    description: >-\n      Short-lived launch token minted by the launch endpoint and returned to the\n      SDK via the fetchClientSecrets() callback. The SDK exchanges it to load and\n      authenticate the embedded app. Tokens expire after 5 minutes and must be\n      requested fresh per session.\nenvironments:\n  production: https://api.tortus.ai\n  sandbox: https://api.staging.tortus.ai\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tortus/refs/heads/main/authentication/tortus-authentication.yml
summary_line: http-basic/publishable-key/launch-token · 3 schemes
tags:
- Company
- Healthcare
- Artificial Intelligence
- Ambient Clinical Documentation
- Medical Scribe
- Speech to Text
- EHR Integration
- NHS
- Embed SDK
---
