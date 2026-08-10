---
api_key_in:
- header
api_specs:
- filename: securitize-apac-api-openapi.yml
  format: yaml
  label: Securitize APAC API
  slug: securitize-apac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-apac-api-openapi.yml
- filename: securitize-domains-api-openapi.yml
  format: yaml
  label: Securitize Domains API
  slug: securitize-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-domains-api-openapi.yml
- filename: securitize-health-check-api-openapi.yml
  format: yaml
  label: Securitize Health Check API
  slug: securitize-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-health-check-api-openapi.yml
- filename: securitize-travel-rule-api-openapi.yml
  format: yaml
  label: Securitize Travel Rule API
  slug: securitize-travel-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-travel-rule-api-openapi.yml
- filename: securitize-webhooks-api-openapi.yml
  format: yaml
  label: Securitize Webhooks API
  slug: securitize-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Securitize Authentication
name_suffix: Authentication
oauth_flows: []
overview: Securitize secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Securitize
provider_slug: securitize
scheme_count: 1
schemes:
- description: API Key Format as "apiKey &lt;key_id&gt;:&lt;key_secret&gt;"
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/securitize-domains-openapi-original.json
  type: apiKey
slug: securitize-authentication
source_filename: securitize-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: openapi/securitize-domains-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API Key Format as \"apiKey &lt;key_id&gt;:&lt;key_secret&gt;\"\n  sources:\n  - openapi/securitize-domains-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/authentication/securitize-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- tokenization
- digital-securities
- real-world-assets
- capital-markets
- fund-administration
- transfer-agent
- kyc
- aml
- identity-verification
- blockchain
- broker-dealer
- private-credit
- mcp
- webhooks
---
