---
api_key_in:
- header
api_specs:
- filename: cofactr-knowledge-graph-openapi-original.json
  format: json
  label: Cofactr Knowledge Graph (Component Cloud) API
  slug: cofactr-knowledge-graph-component-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cofactr/refs/heads/main/openapi/cofactr-knowledge-graph-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cofactr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cofactr secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cofactr
provider_slug: cofactr
scheme_count: 3
schemes:
- api: Cofactr Platform API
  case_sensitive: true
  description: 'Platform API (flagship-api.cofactr.com) authenticates with a case-sensitive "Authorization: Api-Key <key>" header. Keys are generated in the platform.'
  format: Api-Key <key>
  in: header
  keys_url: https://platform.cofactr.com/integrations/api-keys
  name: PlatformApiKey
  parameter: Authorization
  sources:
  - https://support.cofactr.com/articles/4081898446-cofactr-platform-api-documentation
  type: apiKey
- description: Issued with your client ID as one Cofactr credential set. Never expose your API key in front-end code or public Git repositories. The Cofactr API is for server-side use only. Public disclosure of a key results in immediate revocation without prior warning.
  in: header
  name: ApiKey
  parameter: X-API-KEY
  sources:
  - openapi/cofactr-knowledge-graph-openapi-original.json
  type: apiKey
- description: Issued with your API key as one Cofactr credential set.
  in: header
  name: ClientId
  parameter: X-CLIENT-ID
  sources:
  - openapi/cofactr-knowledge-graph-openapi-original.json
  type: apiKey
slug: cofactr-authentication
source_filename: cofactr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cofactr-knowledge-graph-openapi-original.json\ndocs: https://support.cofactr.com/collections/5590442793-developer_resources\nkeys_url: https://platform.cofactr.com/integrations/api-keys\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  apis:\n    Cofactr Knowledge Graph: X-CLIENT-ID + X-API-KEY headers (one credential set, server-side only)\n    Cofactr Platform API: \"Authorization: Api-Key <key> (case-sensitive)\"\n  sso: SAML SSO available for the platform (support KB \"Configuring SAML SSO\")\nschemes:\n- name: PlatformApiKey\n  api: Cofactr Platform API\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: \"Api-Key <key>\"\n  case_sensitive: true\n  keys_url: https://platform.cofactr.com/integrations/api-keys\n  description: >-\n    Platform API (flagship-api.cofactr.com) authenticates with a case-sensitive\n    \"Authorization: Api-Key <key>\" header. Keys are generated in the platform.\n\
  \  sources:\n  - https://support.cofactr.com/articles/4081898446-cofactr-platform-api-documentation\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Issued with your client ID as one Cofactr credential set. Never expose your API\n    key in front-end code or public Git repositories. The Cofactr API is for server-side use\n    only. Public disclosure of a key results in immediate revocation without prior warning.\n  sources:\n  - openapi/cofactr-knowledge-graph-openapi-original.json\n- name: ClientId\n  type: apiKey\n  in: header\n  parameter: X-CLIENT-ID\n  description: Issued with your API key as one Cofactr credential set.\n  sources:\n  - openapi/cofactr-knowledge-graph-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cofactr/refs/heads/main/authentication/cofactr-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Physical Ai
- Component Intelligence
- Electronics
- Supply Chain
- Procurement
- Manufacturing
- Hardware
- Bill Of Materials
---
