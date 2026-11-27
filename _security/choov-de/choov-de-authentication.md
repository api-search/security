---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Choov Authentication
name_suffix: Authentication
oauth_flows: []
overview: Choov declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Choov
provider_slug: choov-de
scheme_count: 1
schemes:
- applies_to: https://www.choov.de/mcp.php
  description: The public MCP server needs no credentials. The site states the comparison is used "ohne Registrierung" and "Kein Account", and the setup instructions only give the server URL (claude mcp add --transport http choov https://www.choov.de/mcp.php) with no key or OAuth step.
  evidence: Nein. Choov ist für Nutzer vollständig kostenlos und erfordert keine Registrierung.
  name: none
  type: none
slug: choov-de-authentication
source_filename: choov-de-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Choov authentication\ngenerated: '2026-11-03'\nmethod: searched\nsource: https://choov.de/faq.html\ndocs: https://choov.de/\nschemes:\n- name: none\n  type: none\n  applies_to: https://www.choov.de/mcp.php\n  description: The public MCP server needs no credentials. The site states the comparison is used \"ohne Registrierung\" and \"Kein Account\", and the setup instructions only give the server URL (claude mcp add --transport http choov https://www.choov.de/mcp.php) with no key or OAuth step.\n  evidence: \"Nein. Choov ist für Nutzer vollständig kostenlos und erfordert keine Registrierung.\"\nnote: The FAQ also mentions a partner \"Import-Endpunkt\" and a \"Partnerportal\" that admitted tariff providers get access to after onboarding. Their authentication is not documented in public, and neither was probed.\n"
source_yaml_url: https://artifacts.apis.io/choov-de/authentication/choov-de-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Energy
- Electricity
- Tariff Comparison
- MCP
- AI Agents
- Marketplace
- Germany
---
