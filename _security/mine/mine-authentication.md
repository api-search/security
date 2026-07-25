---
api_key_in:
- header
api_specs:
- filename: mine-aispm-api-openapi.yml
  format: yaml
  label: MINE Aispm API
  slug: mine-aispm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-aispm-api-openapi.yml
- filename: mine-aispmdeviceflags-api-openapi.yml
  format: yaml
  label: MINE AispmDeviceFlags API
  slug: mine-aispmdeviceflags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-aispmdeviceflags-api-openapi.yml
- filename: mine-aispmenroll-api-openapi.yml
  format: yaml
  label: MINE AispmEnroll API
  slug: mine-aispmenroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-aispmenroll-api-openapi.yml
- filename: mine-aispmenrollmenttokens-api-openapi.yml
  format: yaml
  label: MINE AispmEnrollmentTokens API
  slug: mine-aispmenrollmenttokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-aispmenrollmenttokens-api-openapi.yml
- filename: mine-aispmingest-api-openapi.yml
  format: yaml
  label: MINE AispmIngest API
  slug: mine-aispmingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-aispmingest-api-openapi.yml
- filename: mine-aispminsights-api-openapi.yml
  format: yaml
  label: MINE AispmInsights API
  slug: mine-aispminsights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-aispminsights-api-openapi.yml
- filename: mine-aispmpublicagents-api-openapi.yml
  format: yaml
  label: MINE AispmPublicAgents API
  slug: mine-aispmpublicagents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-aispmpublicagents-api-openapi.yml
- filename: mine-aispmpublicdevices-api-openapi.yml
  format: yaml
  label: MINE AispmPublicDevices API
  slug: mine-aispmpublicdevices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-aispmpublicdevices-api-openapi.yml
- filename: mine-assessment-api-openapi.yml
  format: yaml
  label: MINE Assessment API
  slug: mine-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-assessment-api-openapi.yml
- filename: mine-assessmenttemplate-api-openapi.yml
  format: yaml
  label: MINE AssessmentTemplate API
  slug: mine-assessmenttemplate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-assessmenttemplate-api-openapi.yml
- filename: mine-employee-api-openapi.yml
  format: yaml
  label: MINE Employee API
  slug: mine-employee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-employee-api-openapi.yml
- filename: mine-evidencesearch-api-openapi.yml
  format: yaml
  label: MINE EvidenceSearch API
  slug: mine-evidencesearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-evidencesearch-api-openapi.yml
- filename: mine-partners-api-openapi.yml
  format: yaml
  label: MINE Partners API
  slug: mine-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-partners-api-openapi.yml
- filename: mine-privacyrightspublic-api-openapi.yml
  format: yaml
  label: MINE PrivacyRightsPublic API
  slug: mine-privacyrightspublic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-privacyrightspublic-api-openapi.yml
- filename: mine-system-api-openapi.yml
  format: yaml
  label: MINE System API
  slug: mine-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-system-api-openapi.yml
- filename: mine-test-api-openapi.yml
  format: yaml
  label: MINE Test API
  slug: mine-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-test-api-openapi.yml
- filename: mine-tickets-api-openapi.yml
  format: yaml
  label: MINE Tickets API
  slug: mine-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-tickets-api-openapi.yml
- filename: mine-webhooks-api-openapi.yml
  format: yaml
  label: MINE Webhooks API
  slug: mine-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mine Authentication
name_suffix: Authentication
oauth_flows: []
overview: MINE secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MINE
provider_slug: mine
scheme_count: 1
schemes:
- description: "Authorization header using the Bearer scheme. \r\n\r\nEnter 'Bearer' [space] and then your API Key in the text input below.\r\n\r\nExample: 'Bearer 12345abcdef'"
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/mine-openapi-original.json
  - openapi/mine-partners-openapi-original.json
  type: apiKey
slug: mine-authentication
source_filename: mine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/mine-openapi-original.json, openapi/mine-partners-openapi-original.json\ndocs: https://developers.mineos.ai/docs/authentication\nnotes: >-\n  API-key Bearer token. Create keys in the workspace under For Developers > API Keys;\n  the key is shown once. Max 10 active keys per workspace. HTTPS is required.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: \"Authorization header using the Bearer scheme. \\r\\n\\r\\nEnter 'Bearer' [space]\\\n    \\ and then your API Key in the text input below.\\r\\n\\r\\nExample: 'Bearer 12345abcdef'\"\n  sources:\n  - openapi/mine-openapi-original.json\n  - openapi/mine-partners-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/authentication/mine-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data Privacy
- Data Governance
- Privacy Operations
- Consent Management
- AI Governance
- Third-Party Risk
- Compliance
- Security
---
