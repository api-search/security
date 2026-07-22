---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Slashnext Authentication
name_suffix: Authentication
oauth_flows: []
overview: SlashNext secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SlashNext
provider_slug: slashnext
scheme_count: 1
schemes:
- description: Per-tenant SlashNext OTI API key. Sent with each request to https://oti.slashnext.cloud/api/ endpoints. Missing/invalid keys return the SlashNext error envelope {"errorNo","errorMsg"}.
  in: query
  name: authkey
  parameter: authkey
  sources:
  - docs
  type: apiKey
slug: slashnext-authentication
source_filename: slashnext-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://xsoar.pan.dev/docs/reference/integrations/slash-next-phishing-incident-response\ndocs: https://techdocs.cyware.com/co/en/slashnext-threat-intelligence.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  api_key_param: authkey\n  oauth2_flows: []\n  notes: >-\n    The SlashNext On-demand Threat Intelligence (OTI) REST API authenticates\n    every request with a per-tenant API key passed as the `authkey` parameter.\n    No OAuth2 / OpenID Connect surface is documented. The API key is issued by\n    SlashNext (now Varonis) and scoped to the tenant's quota tier.\nschemes:\n- name: authkey\n  type: apiKey\n  in: query\n  parameter: authkey\n  description: >-\n    Per-tenant SlashNext OTI API key. Sent with each request to\n    https://oti.slashnext.cloud/api/ endpoints. Missing/invalid keys return the\n    SlashNext error envelope {\"errorNo\",\"errorMsg\"}.\n  sources:\n  - docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slashnext/refs/heads/main/authentication/slashnext-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Phishing
- Threat Intelligence
- Email Security
- Anti-Phishing
- API
---
