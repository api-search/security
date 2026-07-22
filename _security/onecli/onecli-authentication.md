---
api_key_in: []
api_specs:
- filename: onecli-openapi-original.yml
  format: yaml
  label: OneCLI API
  slug: onecli-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onecli/refs/heads/main/openapi/onecli-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Onecli Authentication
name_suffix: Authentication
oauth_flows: []
overview: Onecli secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Onecli
provider_slug: onecli
scheme_count: 1
schemes:
- description: 'API key obtained from the OneCLI dashboard or `GET /v1/user/api-key`, sent as `Authorization: Bearer <key>`. Cookie-based dashboard sessions are also accepted.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/onecli-openapi-original.yml
  type: http
slug: onecli-authentication
source_filename: onecli-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/onecli-openapi-original.yml\ndocs: https://onecli.sh/docs/api-reference\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_prefixes:\n  - oc_          # project-scoped key\n  - oc_org_      # organization-scoped key (requires X-Project-Id for project endpoints)\n  - oc_partner_  # partner-scoped key (reseller / agency provisioning)\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API key obtained from the OneCLI dashboard or `GET /v1/user/api-key`, sent as\n    `Authorization: Bearer <key>`. Cookie-based dashboard sessions are also accepted.\n  sources:\n  - openapi/onecli-openapi-original.yml\nnotes:\n- \"All endpoints require authentication.\"\n- \"Project keys (oc_) operate on a single project.\"\n- \"Organization keys (oc_org_) can operate across projects; project-scoped endpoints require an X-Project-Id: proj_... header (a 401 is returned without it).\"\n\
  - \"Organization endpoints (/org/...) need no project header and require the admin or owner role, except GET /org/rules/permissions/{provider} which any member may read.\"\n- \"Partner keys (oc_partner_) provision and manage organizations on behalf of customers.\"\n- \"OAuth is used by the gateway to connect downstream apps (Google, GitHub, Slack, ...), not to authenticate to the OneCLI management API itself.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onecli/refs/heads/main/authentication/onecli-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Identity
- AI Agents
- Secrets Management
- Credentials
- Gateway
- OAuth
- Developer Tools
- MCP
- Vault
---
