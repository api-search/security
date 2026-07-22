---
api_key_in:
- unknown
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dropsuite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dropsuite secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dropsuite
provider_slug: dropsuite
scheme_count: 2
schemes:
- description: Partner reseller token issued in the Partner Portal (Settings -> API Settings).
  name: ResellerToken
  sources:
  - docs
  type: apiKey
- description: Authentication token issued in the Partner Portal (Settings -> API Settings).
  name: AuthenticationToken
  sources:
  - docs
  type: apiKey
slug: dropsuite-authentication
source_filename: dropsuite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://help.dropsuite.com/hc/en-us/articles/20422080552855-15-API-Settings\ndocs: https://help.dropsuite.com/hc/en-us/articles/20422080552855-15-API-Settings\nnotes: >-\n  Dropsuite (now NinjaOne SaaS Backup) exposes a partner REST API whose credentials\n  are provisioned per-partner from the Partner Portal under Settings -> API Settings.\n  API access is gated to Direct Partners / Distributors. No public OpenAPI or open\n  self-service credentials are published; the API URL is partner-specific. Auth is\n  token-based using two tokens issued in the portal (Reseller Token + Authentication\n  Token) alongside the partner API URL. Exact header/parameter names are documented\n  inside the partner-gated help center and are not reproduced here (no fabrication).\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - unknown\n  oauth2_flows: []\n  access: partner-gated\nschemes:\n- name: ResellerToken\n  type: apiKey\n  description:\
  \ Partner reseller token issued in the Partner Portal (Settings -> API Settings).\n  sources:\n  - docs\n- name: AuthenticationToken\n  type: apiKey\n  description: Authentication token issued in the Partner Portal (Settings -> API Settings).\n  sources:\n  - docs\nreferences:\n- https://help.dropsuite.com/hc/en-us/articles/38775854335895-API-Authentication-for-Rewst-Integration\n- https://help.dropsuite.com/hc/en-us/articles/16883894866587\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dropsuite/refs/heads/main/authentication/dropsuite-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Cloud Backup
- Data Protection
- Email Archiving
- Microsoft 365
- Google Workspace
- MSP
- Compliance
- eDiscovery
- Disaster Recovery
---
