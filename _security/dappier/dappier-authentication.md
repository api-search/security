---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dappier-app-api-openapi.yml
  format: yaml
  label: Dappier App API
  slug: dappier-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dappier/refs/heads/main/openapi/dappier-app-api-openapi.yml
auth_types: []
description: Authentication for Dappier API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dappier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dappier declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dappier
provider_slug: dappier
scheme_count: 1
schemes:
- evidence: 'headers = {"Authorization": f"Bearer {api_key}", "Content-Type": "application/json"}'
  header: Authorization
  how_to_obtain: Obtain API key from Dappier Platform under Settings > Profile > API Keys.
  location: header
  name: Bearer
  type: http-bearer
slug: dappier-authentication
source_filename: dappier-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.dappier.com/quickstart.md
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.dappier.com/quickstart.md\nsources:\n- https://docs.dappier.com/quickstart.md\ndescription: Authentication for Dappier API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'headers = {\"Authorization\": f\"Bearer {api_key}\", \"Content-Type\": \"application/json\"}'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain API key from Dappier Platform under Settings > Profile > API Keys.\ndocs: https://docs.dappier.com/quickstart.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dappier/refs/heads/main/authentication/dappier-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Advertising
- Monetization
- Publishers
---
