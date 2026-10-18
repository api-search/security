---
anonymous_access: false
api_key_in: []
api_specs:
- filename: connectly-businesses-api-openapi.yml
  format: yaml
  label: Connectly Businesses API
  slug: connectly-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connectly/refs/heads/main/openapi/connectly-businesses-api-openapi.yml
auth_types: []
description: API keys authenticate your requests to the Connectly API.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Connectly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Connectly declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Connectly
provider_slug: connectly
scheme_count: 1
schemes:
- evidence: 'Include the key in the `X-API-Key` header on every request to the Connectly API:'
  header: X-API-Key
  how_to_obtain: Generate and manage API keys from the Connectly Settings page — with scoped permissions and optional expiration.
  location: header
  name: API Key
  scopes:
  - ai.manage
  - campaign.manage
  - commerce.manage
  - conversation.manage
  - customer.manage
  - key.manage
  - messaging.send
  - system.manage
  - workspace.manage
  type: apiKey
slug: connectly-authentication
source_filename: connectly-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.connectly.ai/get-started/authentication-and-api-keys.md
source_yaml: "generated: '2026-10-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.connectly.ai/get-started/authentication-and-api-keys.md\nsources:\n- https://docs.connectly.ai/get-started/authentication-and-api-keys.md\n- https://docs.connectly.ai/get-started/quick-start.md\n- https://docs.connectly.ai/business-hub/campaigns/ctwa.md\ndescription: API keys authenticate your requests to the Connectly API.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Include the key in the `X-API-Key` header on every request to the Connectly API:'\n  location: header\n  header: X-API-Key\n  scopes:\n  - ai.manage\n  - campaign.manage\n  - commerce.manage\n  - conversation.manage\n  - customer.manage\n  - key.manage\n  - messaging.send\n  - system.manage\n  - workspace.manage\n  how_to_obtain: Generate and manage API keys from the Connectly Settings page — with scoped permissions and optional expiration.\ndocs: https://docs.connectly.ai/get-started/authentication-and-api-keys.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connectly/refs/heads/main/authentication/connectly-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Platform
- CustomerEngagement
- Enterprise
- Automation
---
