---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes supported by APIANT as described in the documentation.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Apiant Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIANT declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: APIANT
provider_slug: apiant
scheme_count: 2
schemes:
- evidence: API Key — a single token (or username/password pair) you paste into the keyvault when Claude prompts you.
  how_to_obtain: Paste the key into the connection‑manager page that Claude opens.
  name: API Key
  type: apiKey
- evidence: OAuth V2 — a multi‑step flow where you register a developer application with the service.
  how_to_obtain: Register a developer application with the vendor, then use the Connect flow guided by Claude.
  name: OAuth V2
  type: oauth2
slug: apiant-authentication
source_filename: apiant-authentication.yml
source_heading: Authentication Profile
source_url: https://info.apiant.com/docs/get-started/api-authentication
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://info.apiant.com/docs/get-started/api-authentication\nsources:\n- https://info.apiant.com/docs/get-started/api-authentication\n- https://info.apiant.com/docs/building-with-the-plugin/connector\n- https://help.apiant.com/automationeditor-multi-factor-authentication\n- https://info.apiant.com/docs/apiant-inline/embed-inline\ndescription: Authentication schemes supported by APIANT as described in the documentation.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: API Key — a single token (or username/password pair) you paste into the keyvault when Claude prompts you.\n  how_to_obtain: Paste the key into the connection‑manager page that Claude opens.\n- type: oauth2\n  name: OAuth V2\n  evidence: OAuth V2 — a multi‑step flow where you register a developer application with the service.\n  how_to_obtain: Register a developer application with the vendor, then use the Connect\
  \ flow guided by Claude.\ndocs: https://info.apiant.com/docs/get-started/api-authentication\n"
source_yaml_url: https://artifacts.apis.io/apiant/authentication/apiant-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Integration
- AI
- Automation
- SaaS
---
