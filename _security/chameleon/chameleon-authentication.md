---
api_key_in:
- header
api_specs:
- filename: chameleon-alert-groups-api-openapi.yml
  format: yaml
  label: Chameleon Alert Groups API
  slug: chameleon-alert-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-alert-groups-api-openapi.yml
- filename: chameleon-companies-api-openapi.yml
  format: yaml
  label: Chameleon Companies API
  slug: chameleon-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-companies-api-openapi.yml
- filename: chameleon-deliveries-api-openapi.yml
  format: yaml
  label: Chameleon Deliveries API
  slug: chameleon-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-deliveries-api-openapi.yml
- filename: chameleon-domains-api-openapi.yml
  format: yaml
  label: Chameleon Domains API
  slug: chameleon-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-domains-api-openapi.yml
- filename: chameleon-imports-api-openapi.yml
  format: yaml
  label: Chameleon Imports API
  slug: chameleon-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-imports-api-openapi.yml
- filename: chameleon-interactions-api-openapi.yml
  format: yaml
  label: Chameleon Interactions API
  slug: chameleon-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-interactions-api-openapi.yml
- filename: chameleon-launchers-api-openapi.yml
  format: yaml
  label: Chameleon Launchers API
  slug: chameleon-launchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-launchers-api-openapi.yml
- filename: chameleon-limit-groups-api-openapi.yml
  format: yaml
  label: Chameleon Limit Groups API
  slug: chameleon-limit-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-limit-groups-api-openapi.yml
- filename: chameleon-microsurveys-api-openapi.yml
  format: yaml
  label: Chameleon Microsurveys API
  slug: chameleon-microsurveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-microsurveys-api-openapi.yml
- filename: chameleon-profiles-api-openapi.yml
  format: yaml
  label: Chameleon Profiles API
  slug: chameleon-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-profiles-api-openapi.yml
- filename: chameleon-properties-api-openapi.yml
  format: yaml
  label: Chameleon Properties API
  slug: chameleon-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-properties-api-openapi.yml
- filename: chameleon-responses-api-openapi.yml
  format: yaml
  label: Chameleon Responses API
  slug: chameleon-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-responses-api-openapi.yml
- filename: chameleon-segments-api-openapi.yml
  format: yaml
  label: Chameleon Segments API
  slug: chameleon-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-segments-api-openapi.yml
- filename: chameleon-tags-api-openapi.yml
  format: yaml
  label: Chameleon Tags API
  slug: chameleon-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-tags-api-openapi.yml
- filename: chameleon-tooltips-api-openapi.yml
  format: yaml
  label: Chameleon Tooltips API
  slug: chameleon-tooltips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-tooltips-api-openapi.yml
- filename: chameleon-tours-api-openapi.yml
  format: yaml
  label: Chameleon Tours API
  slug: chameleon-tours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-tours-api-openapi.yml
- filename: chameleon-webhooks-api-openapi.yml
  format: yaml
  label: Chameleon Webhooks API
  slug: chameleon-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Chameleon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chameleon secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chameleon
provider_slug: chameleon
scheme_count: 1
schemes:
- description: Your Chameleon account secret. See https://developers.chameleon.io/api-introduction/authentication
  in: header
  name: accountSecret
  parameter: X-Account-Secret
  sources:
  - openapi/chameleon-openapi.yml
  type: apiKey
slug: chameleon-authentication
source_filename: chameleon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chameleon-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accountSecret\n  type: apiKey\n  in: header\n  parameter: X-Account-Secret\n  description: Your Chameleon account secret. See https://developers.chameleon.io/api-introduction/authentication\n  sources:\n  - openapi/chameleon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/authentication/chameleon-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Product
- In-App Guidance
- Onboarding
- Surveys
- Analytics
---
