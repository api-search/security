---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses an API token sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: notolens Authentication
name_suffix: Authentication
oauth_flows: []
overview: notolens declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: notolens
provider_slug: notolens-com
scheme_count: 1
schemes:
- evidence: 'The client sends it as `Authorization: Bearer <token>`.'
  header: Authorization
  how_to_obtain: User creates an API token in notolens Settings → API tokens and stores it in the NOTOLENS_API_TOKEN environment variable.
  location: header
  name: Bearer token
  type: http-bearer
slug: notolens-com-authentication
source_filename: notolens-com-authentication.yml
source_heading: Authentication Profile
source_url: https://notolens.com/ai/agent-setup.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://notolens.com/ai/agent-setup.md\nsources:\n- https://notolens.com/ai/agent-setup.md\ndescription: Authentication uses an API token sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'The client sends it as `Authorization: Bearer <token>`.'\n  location: header\n  header: Authorization\n  how_to_obtain: User creates an API token in notolens Settings → API tokens and stores it in the NOTOLENS_API_TOKEN environment variable.\ndocs: https://notolens.com/ai/agent-setup.md\n"
source_yaml_url: https://artifacts.apis.io/notolens-com/authentication/notolens-com-authentication.yml
summary_line: 1 scheme
tags:
- Brand Protection
- Trademark Monitoring
- Domain Monitoring
- App Store Monitoring
- Ad Monitoring
- AI Assessment
---
