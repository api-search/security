---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for MeshArc API uses API keys presented as Bearer tokens.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mesharc Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: mesharc-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mesharc-dev
provider_slug: mesharc-dev
scheme_count: 1
schemes:
- evidence: 'curl https://api.mesharc.dev/api/v1/scrape \ -H "Authorization: Bearer mesharc_..." -H "Content-Type: application/json" \ -d ''{"url": "https://example.com/pricing", "formats": "markdown,links"}'''
  header: Authorization
  how_to_obtain: Settings → API keys → New key. The key is shown once.
  location: header
  name: Bearer
  type: http-bearer
slug: mesharc-dev-authentication
source_filename: mesharc-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://mesharc.dev/docs/getting-started
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mesharc.dev/docs/getting-started\nsources:\n- https://mesharc.dev/docs/getting-started\ndescription: Authentication for MeshArc API uses API keys presented as Bearer tokens.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl https://api.mesharc.dev/api/v1/scrape \\ -H \"Authorization: Bearer mesharc_...\" -H \"Content-Type: application/json\" \\ -d ''{\"url\":\n    \"https://example.com/pricing\", \"formats\": \"markdown,links\"}'''\n  location: header\n  header: Authorization\n  how_to_obtain: Settings → API keys → New key. The key is shown once.\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the page.\ndocs: https://mesharc.dev/docs/getting-started\n"
source_yaml_url: https://artifacts.apis.io/mesharc-dev/authentication/mesharc-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Medical Imaging
- Data Management
- Healthcare
- Developer Tools
---
