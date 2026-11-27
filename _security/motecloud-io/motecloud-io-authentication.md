---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for MoteCloud agents as described on the quickstart page.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: MoteCloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: MoteCloud declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: MoteCloud
provider_slug: motecloud-io
scheme_count: 3
schemes:
- evidence: Use the mtak_... key with X-Tenant-ID and X-Tenant-Token headers.
  header: X-Tenant-Token
  how_to_obtain: Create a direct agent key in /account.
  location: header
  name: mtak
  type: apiKey
- evidence: Use the mtak_... key with X-Tenant-ID and X-Tenant-Token headers.
  header: X-Tenant-ID
  how_to_obtain: Create a direct agent key in /account.
  location: header
  name: tenant-id
  type: apiKey
- evidence: 'Authorization: Bearer ags_... and your tenant ID.'
  header: Authorization
  how_to_obtain: Obtain a one‑time enrollment token in /account or via the wallet challenge flow, then POST /v2/agents/signup.
  location: header
  name: ags
  type: http-bearer
slug: motecloud-io-authentication
source_filename: motecloud-io-authentication.yml
source_heading: Authentication Profile
source_url: https://motecloud.io/agents
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://motecloud.io/agents\nsources:\n- https://motecloud.io/agents\ndescription: Authentication methods for MoteCloud agents as described on the quickstart page.\nschemes:\n- type: apiKey\n  name: mtak\n  evidence: Use the mtak_... key with X-Tenant-ID and X-Tenant-Token headers.\n  location: header\n  header: X-Tenant-Token\n  how_to_obtain: Create a direct agent key in /account.\n- type: apiKey\n  name: tenant-id\n  evidence: Use the mtak_... key with X-Tenant-ID and X-Tenant-Token headers.\n  location: header\n  header: X-Tenant-ID\n  how_to_obtain: Create a direct agent key in /account.\n- type: http-bearer\n  name: ags\n  evidence: 'Authorization: Bearer ags_... and your tenant ID.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a one‑time enrollment token in /account or via the wallet challenge flow, then POST /v2/agents/signup.\nnote: Admin and observability\
  \ routes use JWT‑admin authentication, but the page does not provide details such as header name or token format.\ndocs: https://motecloud.io/agents\n"
source_yaml_url: https://artifacts.apis.io/motecloud-io/authentication/motecloud-io-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- GraphMemory
- Production
- Platform
- MoteCloud
---
