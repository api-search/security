---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication via API key used as a Bearer token or X‑API‑Key header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Clickshealth Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clicks declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Clicks
provider_slug: clickshealth-com
scheme_count: 2
schemes:
- evidence: 'Send the key as a Bearer token on every request:'
  header: Authorization
  how_to_obtain: Create a key in the Clicks app under the agent's API access tab; the full secret is shown once as `ak_…`.
  location: header
  name: Bearer
  type: http-bearer
- evidence: If the `Authorization` header is missing or isn't a Bearer credential, the API also accepts the key in an `X-API-Key` header.
  header: X-API-Key
  how_to_obtain: Create a key in the Clicks app under the agent's API access tab; the full secret is shown once as `ak_…`.
  location: header
  name: X-API-Key
  type: apiKey
slug: clickshealth-com-authentication
source_filename: clickshealth-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.clickshealth.com/authentication.md
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.clickshealth.com/authentication.md\nsources:\n- https://docs.clickshealth.com/authentication.md\n- https://docs.clickshealth.com/quickstart.md\ndescription: Authentication via API key used as a Bearer token or X‑API‑Key header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send the key as a Bearer token on every request:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the Clicks app under the agent's API access tab; the full secret is shown once as `ak_…`.\n- type: apiKey\n  name: X-API-Key\n  evidence: If the `Authorization` header is missing or isn't a Bearer credential, the API also accepts the key in an `X-API-Key` header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a key in the Clicks app under the agent's API access tab; the full secret is shown once as `ak_…`.\ndocs: https://docs.clickshealth.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/clickshealth-com/authentication/clickshealth-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Healthcare
- AI
- Revenue Cycle Management
- Automation
---
