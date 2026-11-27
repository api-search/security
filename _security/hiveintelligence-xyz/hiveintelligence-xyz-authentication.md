---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Hive MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hive Intelligence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hive Intelligence declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hive Intelligence
provider_slug: hiveintelligence-xyz
scheme_count: 2
schemes:
- evidence: Clients like Claude, Cursor, VS Code, and ChatGPT authorize with OAuth in the browser.
  name: OAuth
  type: oauth2
- evidence: 'Cron jobs, backends, and CI have no browser, so they use a key instead:'
  header: Authorization
  how_to_obtain: Create one at https://www.hiveintelligence.xyz/dashboard/keys
  location: header
  name: API key
  type: apiKey
slug: hiveintelligence-xyz-authentication
source_filename: hiveintelligence-xyz-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.hiveintelligence.xyz/authentication.md
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.hiveintelligence.xyz/authentication.md\nsources:\n- https://docs.hiveintelligence.xyz/authentication.md\n- https://docs.hiveintelligence.xyz/guides/token-security.md\n- https://docs.hiveintelligence.xyz/tools/token-contract.md\n- https://docs.hiveintelligence.xyz/tools/security.md\ndescription: Authentication methods for Hive MCP\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Clients like Claude, Cursor, VS Code, and ChatGPT authorize with OAuth in the browser.\n- type: apiKey\n  name: API key\n  evidence: 'Cron jobs, backends, and CI have no browser, so they use a key instead:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create one at https://www.hiveintelligence.xyz/dashboard/keys\ndocs: https://docs.hiveintelligence.xyz/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/hiveintelligence-xyz/authentication/hiveintelligence-xyz-authentication.yml
summary_line: 2 schemes
tags:
- Cryptocurrency
- Artificial Intelligence
- Data
- Markets
- Live
---
