---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Popp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Popp secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Popp
provider_slug: popp
scheme_count: 2
schemes:
- description: Secret key authenticating the request; grants full access to the organization's data.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - https://docs.joinpopp.com/docs/authentication-guide
  type: apiKey
- description: Unique identifier for the caller's subaccount (organization) in Popp; required alongside the API key.
  in: header
  name: OrganizationId
  parameter: x-organization-id
  sources:
  - https://docs.joinpopp.com/docs/authentication-guide
  type: apiKey
slug: popp-authentication
source_filename: popp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.joinpopp.com/docs/authentication-guide\ndocs: https://docs.joinpopp.com/docs/authentication-guide\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    Every request requires TWO headers: a secret API key and the caller's\n    Organization ID. No OAuth or OpenID Connect surface is documented.\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    description: Secret key authenticating the request; grants full access to the organization's data.\n    sources: [https://docs.joinpopp.com/docs/authentication-guide]\n  - name: OrganizationId\n    type: apiKey\n    in: header\n    parameter: x-organization-id\n    description: Unique identifier for the caller's subaccount (organization) in Popp; required alongside the API key.\n    sources: [https://docs.joinpopp.com/docs/authentication-guide]\ncredentials_portal: https://app.joinpopp.com/developer/keys\n\
  key_management:\n  self_serve: true\n  features: [create, expiry, revocation]\n  docs: https://docs.joinpopp.com/docs/api-key-management\nexample_request: |\n  curl -X GET \"https://api.joinpopp.com/v1/conversations\" \\\n    -H \"x-api-key: YOUR_API_KEY\" \\\n    -H \"x-organization-id: YOUR_ORGANIZATION_ID\" \\\n    -H \"Content-Type: application/json\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/authentication/popp-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Recruitment
- Staffing
- Hiring
- Conversational AI
- Automation
- Scheduling
- Workflows
- Webhooks
- MCP
- Agents
---
