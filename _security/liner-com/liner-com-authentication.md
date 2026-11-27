---
anonymous_access: false
api_key_in: []
api_specs:
- filename: liner-com-openapi-generated.yml
  format: yaml
  label: Liner API
  slug: liner-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liner-com/openapi/_ae-authored/liner-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Liner APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Liner Authentication
name_suffix: Authentication
oauth_flows: []
overview: Liner declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Liner
provider_slug: liner-com
scheme_count: 2
schemes:
- evidence: Authenticate with an environment API key, sent in the x-api-key header.
  header: x-api-key
  how_to_obtain: Create a new key in the API Keys section of the Liner Platform and store it as an environment variable.
  location: header
  name: Liner API Key
  type: apiKey
- evidence: 'Once the client has the token, it calls the runtime endpoints with the Authorization: Bearer header and omits externalUserId entirely.'
  header: Authorization
  how_to_obtain: Mint a delegated token via POST https://actions.liner.com/api/v1/platform/delegated‑tokens using an environment API key.
  location: header
  name: Delegated Token
  type: http-bearer
slug: liner-com-authentication
source_filename: liner-com-authentication.yml
source_heading: Authentication Profile
source_url: https://liner.com/developers/docs/quick-start
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://liner.com/developers/docs/quick-start\nsources:\n- https://liner.com/developers/docs/quick-start\n- https://liner.com/developers/docs/actions-api-delegated-tokens-create\n- https://liner.com/developers/docs/router-api\n- https://liner.com/developers/docs/pricing\ndescription: Authentication methods for Liner APIs\nschemes:\n- type: apiKey\n  name: Liner API Key\n  evidence: Authenticate with an environment API key, sent in the x-api-key header.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a new key in the API Keys section of the Liner Platform and store it as an environment variable.\n- type: http-bearer\n  name: Delegated Token\n  evidence: 'Once the client has the token, it calls the runtime endpoints with the Authorization: Bearer header and omits externalUserId entirely.'\n  location: header\n  header: Authorization\n  how_to_obtain: Mint a delegated\
  \ token via POST https://actions.liner.com/api/v1/platform/delegated‑tokens using an environment API key.\ndocs: https://liner.com/developers/docs/quick-start\n"
source_yaml_url: https://artifacts.apis.io/liner-com/authentication/liner-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Research
- Agents
- Platform
- Productivity
---
