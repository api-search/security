---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nusii-com-api-v2-account-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Account API
  slug: nusii-com-api-v2-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-account-api-openapi.yml
- filename: nusii-com-api-v2-client-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Client API
  slug: nusii-com-api-v2-client-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-client-api-openapi.yml
- filename: nusii-com-api-v2-currency-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Currency API
  slug: nusii-com-api-v2-currency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-currency-api-openapi.yml
- filename: nusii-com-api-v2-integrations-lessannoyingcrminstallation-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Integrations::Less Annoying CRM Installation API
  slug: nusii-com-api-v2-integrations-lessannoyingcrminstallation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-integrations-lessannoyingcrminstallation-api-openapi.yml
- filename: nusii-com-api-v2-integrations-onepagecrminstallation-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Integrations::One Page CRM Installation API
  slug: nusii-com-api-v2-integrations-onepagecrminstallation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-integrations-onepagecrminstallation-api-openapi.yml
- filename: nusii-com-api-v2-lineitem-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Line Item API
  slug: nusii-com-api-v2-lineitem-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-lineitem-api-openapi.yml
- filename: nusii-com-api-v2-locale-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Locale API
  slug: nusii-com-api-v2-locale-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-locale-api-openapi.yml
- filename: nusii-com-api-v2-pdfpagesize-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Pdf Page Size API
  slug: nusii-com-api-v2-pdfpagesize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-pdfpagesize-api-openapi.yml
- filename: nusii-com-api-v2-proposal-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Proposal API
  slug: nusii-com-api-v2-proposal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-proposal-api-openapi.yml
- filename: nusii-com-api-v2-proposalactivity-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Proposal Activity API
  slug: nusii-com-api-v2-proposalactivity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-proposalactivity-api-openapi.yml
- filename: nusii-com-api-v2-section-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Section API
  slug: nusii-com-api-v2-section-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-section-api-openapi.yml
- filename: nusii-com-api-v2-taxation-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Taxation API
  slug: nusii-com-api-v2-taxation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-taxation-api-openapi.yml
- filename: nusii-com-api-v2-template-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Template API
  slug: nusii-com-api-v2-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-template-api-openapi.yml
- filename: nusii-com-api-v2-theme-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Theme API
  slug: nusii-com-api-v2-theme-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-theme-api-openapi.yml
- filename: nusii-com-api-v2-user-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::User API
  slug: nusii-com-api-v2-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-user-api-openapi.yml
- filename: nusii-com-api-v2-webhook-endpoint-api-openapi.yml
  format: yaml
  label: Nusii Api::V2::Webhook::Endpoint API
  slug: nusii-com-api-v2-webhook-endpoint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nusii-com/openapi/nusii-com-api-v2-webhook-endpoint-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Nusii Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nusii secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nusii
provider_slug: nusii-com
scheme_count: 2
schemes:
- description: 'API key authentication: `Authorization: Token token=YOUR_API_KEY`'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/nusii-com-openapi.yaml
  type: apiKey
- description: OAuth 2.0 access token
  name: OAuthBearer
  scheme: bearer
  sources:
  - openapi/nusii-com-openapi.yaml
  type: http
slug: nusii-com-authentication
source_filename: nusii-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nusii-com-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key authentication: `Authorization: Token token=YOUR_API_KEY`'\n  sources:\n  - openapi/nusii-com-openapi.yaml\n- name: OAuthBearer\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token\n  sources:\n  - openapi/nusii-com-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/nusii-com/authentication/nusii-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Proposal Software
- Software-as-a-Service
- Marketing Agencies
- Service Companies
---
