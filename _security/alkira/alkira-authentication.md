---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Alkira Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alkira secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Alkira
provider_slug: alkira
scheme_count: 2
schemes:
- env_vars:
  - ALKIRA_PORTAL
  - ALKIRA_API_KEY
  format: api-key <base64(API_KEY)>
  in: header
  name: apiKey
  parameter_name: Authorization
  primary: true
  provisioning: Portal > Settings > User Management (per-user key)
  type: apiKey
- deprecated: true
  deprecation_note: Username/password authentication (ALKIRA_USERNAME / ALKIRA_PASSWORD) is deprecated and will be removed in a future major release; migrate to API key auth.
  name: legacy-basic
  scheme: basic
  type: http
slug: alkira-authentication
source_filename: alkira-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://registry.terraform.io/providers/alkiranet/alkira/latest/docs\n# Derived from Alkira's official Terraform provider docs and the client-go client\n# implementation (github.com/alkiranet/client-go, vendored in alkiranet/mcp-alkira).\ndocs: https://registry.terraform.io/providers/alkiranet/alkira/latest/docs\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  header: Authorization\n  scheme_note: 'API key is base64-encoded and prefixed: Authorization: api-key <base64(api_key)>'\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  format: 'api-key <base64(API_KEY)>'\n  provisioning: Portal > Settings > User Management (per-user key)\n  env_vars: [ALKIRA_PORTAL, ALKIRA_API_KEY]\n  primary: true\n- name: legacy-basic\n  type: http\n  scheme: basic\n  deprecated: true\n  deprecation_note: 'Username/password authentication (ALKIRA_USERNAME / ALKIRA_PASSWORD)\n    is deprecated and will\
  \ be removed in a future major release; migrate to API key auth.'\nnotes:\n- Auth is tenant-scoped by the portal host (<tenant>.portal.alkira.com); the client\n  resolves the tenant network id via GET /api/tenantnetworksummaries after auth.\n- No OAuth2/OIDC surface is documented; there is no scope model (skip scopes/).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alkira/refs/heads/main/authentication/alkira-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Enterprise
- Networking
- Cloud
- Multi-Cloud
- Infrastructure
- Network as a Service
- SD-WAN
- Security
- Automation
---
