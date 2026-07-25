---
api_key_in:
- query
api_specs:
- filename: roku-apps-api-openapi.yml
  format: yaml
  label: Roku Apps API
  slug: roku-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-apps-api-openapi.yml
- filename: roku-asyncapi-api-openapi.yml
  format: yaml
  label: Roku asyncapi API
  slug: roku-asyncapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-asyncapi-api-openapi.yml
- filename: roku-billing-api-openapi.yml
  format: yaml
  label: Roku Billing API
  slug: roku-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-billing-api-openapi.yml
- filename: roku-builds-api-openapi.yml
  format: yaml
  label: Roku builds API
  slug: roku-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-builds-api-openapi.yml
- filename: roku-devices-api-openapi.yml
  format: yaml
  label: Roku devices API
  slug: roku-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-devices-api-openapi.yml
- filename: roku-diagnostics-api-openapi.yml
  format: yaml
  label: Roku Diagnostics API
  slug: roku-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-diagnostics-api-openapi.yml
- filename: roku-discovery-api-openapi.yml
  format: yaml
  label: Roku Discovery API
  slug: roku-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-discovery-api-openapi.yml
- filename: roku-groups-api-openapi.yml
  format: yaml
  label: Roku groups API
  slug: roku-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-groups-api-openapi.yml
- filename: roku-healthz-api-openapi.yml
  format: yaml
  label: Roku healthz API
  slug: roku-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-healthz-api-openapi.yml
- filename: roku-input-api-openapi.yml
  format: yaml
  label: Roku Input API
  slug: roku-input-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-input-api-openapi.yml
- filename: roku-keypress-api-openapi.yml
  format: yaml
  label: Roku KeyPress API
  slug: roku-keypress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-keypress-api-openapi.yml
- filename: roku-organisation-roles-api-openapi.yml
  format: yaml
  label: Roku organisation-roles API
  slug: roku-organisation-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-organisation-roles-api-openapi.yml
- filename: roku-organisations-api-openapi.yml
  format: yaml
  label: Roku organisations API
  slug: roku-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-organisations-api-openapi.yml
- filename: roku-personal-access-tokens-api-openapi.yml
  format: yaml
  label: Roku personal-access-tokens API
  slug: roku-personal-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-personal-access-tokens-api-openapi.yml
- filename: roku-projects-api-openapi.yml
  format: yaml
  label: Roku projects API
  slug: roku-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-projects-api-openapi.yml
- filename: roku-query-api-openapi.yml
  format: yaml
  label: Roku Query API
  slug: roku-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-query-api-openapi.yml
- filename: roku-serviceaccounts-api-openapi.yml
  format: yaml
  label: Roku serviceaccounts API
  slug: roku-serviceaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-serviceaccounts-api-openapi.yml
- filename: roku-snapshots-api-openapi.yml
  format: yaml
  label: Roku snapshots API
  slug: roku-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-snapshots-api-openapi.yml
- filename: roku-subscription-api-openapi.yml
  format: yaml
  label: Roku Subscription API
  slug: roku-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-subscription-api-openapi.yml
- filename: roku-users-api-openapi.yml
  format: yaml
  label: Roku users API
  slug: roku-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-users-api-openapi.yml
- filename: roku-validation-api-openapi.yml
  format: yaml
  label: Roku Validation API
  slug: roku-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-validation-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Roku Authentication
name_suffix: Authentication
oauth_flows: []
overview: Roku secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Roku
provider_slug: roku
scheme_count: 1
schemes:
- description: 'Roku-issued Partner API Key. For GET endpoints the key is included in the URL path; for

    POST endpoints it is included in the request body. Channels obtain this key from the Roku

    Developer Dashboard.'
  in: query
  name: PartnerAPIKey
  parameter: partnerAPIKey
  sources:
  - openapi/roku-pay-web-services.yaml
  type: apiKey
slug: roku-authentication
source_filename: roku-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/roku-pay-web-services.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: PartnerAPIKey\n  type: apiKey\n  in: query\n  parameter: partnerAPIKey\n  description: |-\n    Roku-issued Partner API Key. For GET endpoints the key is included in the URL path; for\n    POST endpoints it is included in the request body. Channels obtain this key from the Roku\n    Developer Dashboard.\n  sources:\n  - openapi/roku-pay-web-services.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/authentication/roku-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Streaming
- Television
- Media
- Entertainment
- Connected TV
- Consumer Electronics
---
