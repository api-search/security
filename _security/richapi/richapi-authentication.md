---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses the x-api-key header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Richapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: RichAPI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: RichAPI
provider_slug: richapi
scheme_count: 1
schemes:
- evidence: Authentication uses the x-api-key header.
  header: x-api-key
  location: header
  name: apiKey
  type: apiKey
slug: richapi-authentication
source_filename: richapi-authentication.yml
source_heading: Authentication Profile
source_url: https://richapi.ai/playbooks/per-client-api-keys-for-agencies
source_yaml: "generated: '2026-10-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://richapi.ai/playbooks/per-client-api-keys-for-agencies\nsources:\n- https://richapi.ai/playbooks/per-client-api-keys-for-agencies\ndescription: Authentication uses the x-api-key header.\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: Authentication uses the x-api-key header.\n  location: header\n  header: x-api-key\ndocs: https://richapi.ai/playbooks/per-client-api-keys-for-agencies\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/richapi/refs/heads/main/authentication/richapi-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API
- Data-Enrichment
- B2B
- MCP
---
