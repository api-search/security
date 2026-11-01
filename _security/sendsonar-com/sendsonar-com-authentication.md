---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: sendsonar-com-accounts-api-openapi.yml
  format: yaml
  label: Sonar Accounts API
  slug: sendsonar-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-accounts-api-openapi.yml
- filename: sendsonar-com-campaigns-api-openapi.yml
  format: yaml
  label: Sonar Campaigns API
  slug: sendsonar-com-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-campaigns-api-openapi.yml
- filename: sendsonar-com-conversations-api-openapi.yml
  format: yaml
  label: Sonar Conversations API
  slug: sendsonar-com-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-conversations-api-openapi.yml
- filename: sendsonar-com-customers-api-openapi.yml
  format: yaml
  label: Sonar Customers API
  slug: sendsonar-com-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-customers-api-openapi.yml
- filename: sendsonar-com-events-api-openapi.yml
  format: yaml
  label: Sonar Events API
  slug: sendsonar-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-events-api-openapi.yml
- filename: sendsonar-com-messages-api-openapi.yml
  format: yaml
  label: Sonar Messages API
  slug: sendsonar-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-messages-api-openapi.yml
- filename: sendsonar-com-phone-numbers-api-openapi.yml
  format: yaml
  label: Sonar Phone Numbers API
  slug: sendsonar-com-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-phone-numbers-api-openapi.yml
- filename: sendsonar-com-roles-api-openapi.yml
  format: yaml
  label: Sonar Roles API
  slug: sendsonar-com-roles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-roles-api-openapi.yml
- filename: sendsonar-com-users-api-openapi.yml
  format: yaml
  label: Sonar Users API
  slug: sendsonar-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-users-api-openapi.yml
- filename: sendsonar-com-webhooks-api-openapi.yml
  format: yaml
  label: Sonar Webhooks API
  slug: sendsonar-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Sendsonar Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sonar secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sonar
provider_slug: sendsonar-com
scheme_count: 2
schemes:
- in: header
  name: sec0
  parameter: X-Token
  sources:
  - openapi/sendsonar-com-api-settings-api-openapi.yml
  type: apiKey
- in: query
  name: sec1
  parameter: token
  sources:
  - openapi/sendsonar-com-api-settings-api-openapi.yml
  type: apiKey
slug: sendsonar-com-authentication
source_filename: sendsonar-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: derived\nsource: openapi/sendsonar-com-api-settings-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: X-Token\n  sources:\n  - openapi/sendsonar-com-api-settings-api-openapi.yml\n- name: sec1\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/sendsonar-com-api-settings-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/sendsonar-com/authentication/sendsonar-com-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- SMS
- Messaging
- Sales
- Automation
---
