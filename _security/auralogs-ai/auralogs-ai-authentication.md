---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods documented for Auralogs SDK ingest and Read API/MCP.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Auralogs Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Auralogs declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Auralogs
provider_slug: auralogs-ai
scheme_count: 2
schemes:
- evidence: 'init ({ apiKey: " aura_your_ingest_key " , environment: " production " , });'
  how_to_obtain: Copy the one‑time startup ingest key from the project startup modal.
  name: apiKey
  type: apiKey
- evidence: 'Authorization: Bearer aura_read_YOUR_KEY'
  header: Authorization
  how_to_obtain: Create a read key in the dashboard under Settings → API & MCP keys and copy the plaintext key (aura_read_…).
  location: header
  name: Authorization
  type: http-bearer
slug: auralogs-ai-authentication
source_filename: auralogs-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.auralogs.ai/getting-started/quick-start/
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.auralogs.ai/getting-started/quick-start/\nsources:\n- https://docs.auralogs.ai/getting-started/quick-start/\n- https://docs.auralogs.ai/getting-started/your-first-log/\n- https://docs.auralogs.ai/read-api/setup/\ndescription: Authentication methods documented for Auralogs SDK ingest and Read API/MCP.\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: 'init ({ apiKey: \" aura_your_ingest_key \" , environment: \" production \" , });'\n  how_to_obtain: Copy the one‑time startup ingest key from the project startup modal.\n- type: http-bearer\n  name: Authorization\n  evidence: 'Authorization: Bearer aura_read_YOUR_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a read key in the dashboard under Settings → API & MCP keys and copy the plaintext key (aura_read_…).\ndocs: https://docs.auralogs.ai/getting-started/quick-start/\n"
source_yaml_url: https://artifacts.apis.io/auralogs-ai/authentication/auralogs-ai-authentication.yml
summary_line: 2 schemes
tags:
- Logging
- Artificial Intelligence
- Monitoring
- SDK
- Production
---
