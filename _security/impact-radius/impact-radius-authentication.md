---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Impact Radius Authentication
name_suffix: Authentication
oauth_flows: []
overview: Impact Radius secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Impact Radius
provider_slug: impact-radius
scheme_count: 2
schemes:
- description: Account SID as username, Auth Token as password, base64-encoded in the Authorization header. Applies to Brand, Partner, and Agency REST APIs.
  name: basicAuth
  scheme: basic
  sources:
  - docs
  type: http
- description: Scoped API tokens with fine-grained per-category read/write permissions, created and managed in the impact.com account UI. Presented via the same HTTP Basic Account SID + Auth Token pair.
  in: header
  name: scopedTokens
  sources:
  - docs
  type: apiKey
slug: impact-radius-authentication
source_filename: impact-radius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://integrations.impact.com/rest-apis/api-quick-start/create-an-api-key.md\ndocs: https://integrations.impact.com/rest-apis/api-quick-start.md\nsummary:\n  types: [http]\n  http_scheme: basic\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    REST APIs use HTTP Basic authentication. The Account SID is the username (public\n    identifier, similar to a public key) and the Auth Token is the password (secret\n    credential). The pair is base64-encoded and sent in the Authorization header:\n    `Authorization: Basic base64(AccountSID:AuthToken)`. Access tokens support scoped\n    permissions (\"Scoped Tokens\") with per-category read/write toggles for least-privilege\n    integrations. The hosted MCP server (mcp.impact.com) uses OAuth 2.1 separately.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    Account SID as username, Auth Token as password, base64-encoded in the Authorization\n\
  \    header. Applies to Brand, Partner, and Agency REST APIs.\n  sources: [docs]\n- name: scopedTokens\n  type: apiKey\n  in: header\n  description: >-\n    Scoped API tokens with fine-grained per-category read/write permissions, created and\n    managed in the impact.com account UI. Presented via the same HTTP Basic Account SID +\n    Auth Token pair.\n  sources: [docs]\nbase_urls:\n  brand: https://api.impact.com/Advertisers/{AccountSID}/\n  partner: https://api.impact.com/MediaPartners/{AccountSID}/\n  agency: https://api.impact.com/Agencies/{AccountSID}/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/authentication/impact-radius-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Partnership Management
- Affiliate Marketing
- Influencer Marketing
- Referral Marketing
- Attribution
- Martech
- Advocate
- Creator Economy
- E-Commerce
---
