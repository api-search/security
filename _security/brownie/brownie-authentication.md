---
api_key_in: []
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Brownie Authentication
name_suffix: Authentication
oauth_flows: []
overview: IncidentFox (Brownie) secures its APIs with http and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: IncidentFox (Brownie)
provider_slug: brownie
scheme_count: 3
schemes:
- description: Team token scoped to a single team within an organization. Format "tokid.toksecret" where tokid is the public identifier and toksecret is the secret. Can read/update team configuration, trigger investigations, and view investigation history. Cannot access other teams or modify organization settings. Issued by an organization admin in the Web UI (Admin Console > Teams > Generate Token) and shown once.
  header: 'Authorization: Bearer tokid.toksecret'
  name: teamToken
  scheme: bearer
  type: http
- description: Admin token providing organization-wide access - manage all teams, view audit logs, configure organization settings, and create/revoke team tokens. Format "admin.tokensecret".
  header: 'Authorization: Bearer admin.tokensecret'
  name: adminToken
  scheme: bearer
  type: http
- description: User-based authentication via the organization's identity provider (SSO). Configured in organization settings with issuer, client_id, and client_secret; presented as a standard JWT bearer token.
  name: oidc
  type: openIdConnect
slug: brownie-authentication
source_filename: brownie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.incidentfox.ai/api-reference/authentication\ndocs: https://docs.incidentfox.ai/api-reference/authentication\nsummary:\n  types: [http, openIdConnect]\n  http_schemes: [bearer]\n  transport: Authorization header, Bearer token\nschemes:\n- name: teamToken\n  type: http\n  scheme: bearer\n  description: >-\n    Team token scoped to a single team within an organization. Format\n    \"tokid.toksecret\" where tokid is the public identifier and toksecret is\n    the secret. Can read/update team configuration, trigger investigations,\n    and view investigation history. Cannot access other teams or modify\n    organization settings. Issued by an organization admin in the Web UI\n    (Admin Console > Teams > Generate Token) and shown once.\n  header: 'Authorization: Bearer tokid.toksecret'\n- name: adminToken\n  type: http\n  scheme: bearer\n  description: >-\n    Admin token providing organization-wide access - manage\
  \ all teams, view\n    audit logs, configure organization settings, and create/revoke team\n    tokens. Format \"admin.tokensecret\".\n  header: 'Authorization: Bearer admin.tokensecret'\n- name: oidc\n  type: openIdConnect\n  description: >-\n    User-based authentication via the organization's identity provider (SSO).\n    Configured in organization settings with issuer, client_id, and\n    client_secret; presented as a standard JWT bearer token.\nnotes:\n- All API endpoints require authentication via a Bearer token.\n- Write operations require a team token with write permissions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brownie/refs/heads/main/authentication/brownie-authentication.yml
summary_line: http/openIdConnect · 3 schemes
tags:
- Company
- Incident Response
- SRE
- AIOps
- Observability
- DevOps
- Artificial Intelligence
- Developer Tools
- Automation
- Open Source
---
