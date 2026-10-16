---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses an API key sent in a request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Multion Authentication
name_suffix: Authentication
oauth_flows: []
overview: MultiOn declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MultiOn
provider_slug: multion
scheme_count: 1
schemes:
- evidence: '-H "X_MULTION_API_KEY: MULTION_API_KEY"'
  header: X_MULTION_API_KEY
  how_to_obtain: Create a new API key in the developer console at https://app.multion.ai/api-keys.
  location: header
  name: API key
  type: apiKey
slug: multion-authentication
source_filename: multion-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.multion.ai/quick-start.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.multion.ai/quick-start.md\nsources:\n- https://docs.multion.ai/quick-start.md\ndescription: Authentication uses an API key sent in a request header.\nschemes:\n- type: apiKey\n  name: API key\n  evidence: '-H \"X_MULTION_API_KEY: MULTION_API_KEY\"'\n  location: header\n  header: X_MULTION_API_KEY\n  how_to_obtain: Create a new API key in the developer console at https://app.multion.ai/api-keys.\nnote: No OAuth2 or other authentication schemes are documented on the page.\ndocs: https://docs.multion.ai/quick-start.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/multion/refs/heads/main/authentication/multion-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Automation
- Enterprise
- Platform
---
