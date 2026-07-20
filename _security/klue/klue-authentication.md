---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Klue Authentication
name_suffix: Authentication
oauth_flows: []
overview: Klue secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Klue
provider_slug: klue
scheme_count: 1
schemes:
- applies_to:
  - Klue Content API
  - Klue MCP Server
  description: A Klue API key passed as a Bearer token. Klue's own ChatGPT setup guide instructs users to select "API Key" with "Bearer" as the auth type and paste the Klue API key.
  in: header
  name: klue-content-api-key
  parameter_name: Authorization
  scheme_hint: bearer
  sources:
  - https://klue.com/blog/how-to-connect-klue-to-chatgpt
  type: apiKey
slug: klue-authentication
source_filename: klue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://klue.com/blog/how-to-connect-klue-to-chatgpt\ndocs: https://help.app.klue.com/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    Klue publishes no OpenAPI document publicly; the Content API OpenAPI schema is\n    distributed inside the authenticated application under\n    Apps & Integrations > Content API > \"How to use\". This profile is therefore\n    searched from Klue's public documentation rather than derived from a spec.\nschemes:\n- name: klue-content-api-key\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  scheme_hint: bearer\n  description: >-\n    A Klue API key passed as a Bearer token. Klue's own ChatGPT setup guide\n    instructs users to select \"API Key\" with \"Bearer\" as the auth type and paste\n    the Klue API key.\n  applies_to:\n  - Klue Content API\n  - Klue MCP Server\n  sources:\n  - https://klue.com/blog/how-to-connect-klue-to-chatgpt\n\
  key_management:\n  console_path: Apps & Integrations > Content API > Manage API Keys\n  requires_role: Admin\n  create: Create New API Key\n  named_keys: true\n  expiration:\n    supported: true\n    user_selected: true\n    vendor_recommendation: 1 year for production use\n  rotation_note: >-\n    Keys are named and carry a user-selected expiry, so rotation is\n    self-service. Klue's guidance is to treat the key like a password.\nsso:\n  supported: true\n  protocols: [SAML 2.0]\n  identity_providers:\n  - name: Okta\n    url: https://www.okta.com/integrations/klue/\n  - name: Microsoft Entra ID\n    url: https://learn.microsoft.com/en-us/entra/identity/saas-apps/klue-tutorial\n  source: https://klue.com/product/security\naccess_control:\n  role_based_access: true\n  customized_user_permissions: true\n  source: https://klue.com/product/security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klue/refs/heads/main/authentication/klue-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- SaaS
- Competitive Intelligence
- Competitive Enablement
- Sales Enablement
- Win-Loss Analysis
- Market Intelligence
- Battlecards
- Agents
- MCP
---
