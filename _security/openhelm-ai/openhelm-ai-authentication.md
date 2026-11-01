---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for OpenHelm API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Openhelm Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: openhelm-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: openhelm-ai
provider_slug: openhelm-ai
scheme_count: 1
schemes:
- evidence: 'Every /v1 request authenticates with a Bearer API key. Authorization: Bearer oh_live_...'
  header: Authorization
  how_to_obtain: Mint, name, and revoke keys under Settings → API & Webhooks (org owners/admins).
  location: header
  name: Bearer API key
  type: http-bearer
slug: openhelm-ai-authentication
source_filename: openhelm-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.openhelm.ai/docs/authentication
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.openhelm.ai/docs/authentication\nsources:\n- https://www.openhelm.ai/docs/authentication\n- https://www.openhelm.ai/security\n- https://www.openhelm.ai/docs/installation\n- https://www.openhelm.ai/docs/quick-start\ndescription: Authentication schemes for OpenHelm API\nschemes:\n- type: http-bearer\n  name: Bearer API key\n  evidence: 'Every /v1 request authenticates with a Bearer API key. Authorization: Bearer oh_live_...'\n  location: header\n  header: Authorization\n  how_to_obtain: Mint, name, and revoke keys under Settings → API & Webhooks (org owners/admins).\ndocs: https://www.openhelm.ai/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/openhelm-ai/authentication/openhelm-ai-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Automation
- Productivity
- SaaS
- Platform
---
