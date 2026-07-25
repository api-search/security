---
api_key_in:
- header
api_specs:
- filename: ampersand-api-key-api-openapi.yml
  format: yaml
  label: Ampersand API Key API
  slug: ampersand-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-api-key-api-openapi.yml
- filename: ampersand-billing-account-api-openapi.yml
  format: yaml
  label: Ampersand Billing Account API
  slug: ampersand-billing-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-billing-account-api-openapi.yml
- filename: ampersand-connection-api-openapi.yml
  format: yaml
  label: Ampersand Connection API
  slug: ampersand-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-connection-api-openapi.yml
- filename: ampersand-destination-api-openapi.yml
  format: yaml
  label: Ampersand Destination API
  slug: ampersand-destination-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-destination-api-openapi.yml
- filename: ampersand-installation-api-openapi.yml
  format: yaml
  label: Ampersand Installation API
  slug: ampersand-installation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-installation-api-openapi.yml
- filename: ampersand-integration-api-openapi.yml
  format: yaml
  label: Ampersand Integration API
  slug: ampersand-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-integration-api-openapi.yml
- filename: ampersand-jwt-key-api-openapi.yml
  format: yaml
  label: Ampersand JWT Key API
  slug: ampersand-jwt-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-jwt-key-api-openapi.yml
- filename: ampersand-notification-api-openapi.yml
  format: yaml
  label: Ampersand Notification API
  slug: ampersand-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-notification-api-openapi.yml
- filename: ampersand-oauth-api-openapi.yml
  format: yaml
  label: Ampersand OAuth API
  slug: ampersand-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-oauth-api-openapi.yml
- filename: ampersand-objects-fields-api-openapi.yml
  format: yaml
  label: Ampersand Objects & Fields API
  slug: ampersand-objects-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-objects-fields-api-openapi.yml
- filename: ampersand-operation-api-openapi.yml
  format: yaml
  label: Ampersand Operation API
  slug: ampersand-operation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-operation-api-openapi.yml
- filename: ampersand-org-api-openapi.yml
  format: yaml
  label: Ampersand Org API
  slug: ampersand-org-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-org-api-openapi.yml
- filename: ampersand-project-api-openapi.yml
  format: yaml
  label: Ampersand Project API
  slug: ampersand-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-project-api-openapi.yml
- filename: ampersand-provider-api-openapi.yml
  format: yaml
  label: Ampersand Provider API
  slug: ampersand-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-provider-api-openapi.yml
- filename: ampersand-provider-app-api-openapi.yml
  format: yaml
  label: Ampersand Provider App API
  slug: ampersand-provider-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-provider-app-api-openapi.yml
- filename: ampersand-revision-api-openapi.yml
  format: yaml
  label: Ampersand Revision API
  slug: ampersand-revision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-revision-api-openapi.yml
- filename: ampersand-upload-url-api-openapi.yml
  format: yaml
  label: Ampersand Upload URL API
  slug: ampersand-upload-url-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-upload-url-api-openapi.yml
- filename: ampersand-user-api-openapi.yml
  format: yaml
  label: Ampersand User API
  slug: ampersand-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/openapi/ampersand-user-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ampersand Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ampersand secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ampersand
provider_slug: ampersand
scheme_count: 2
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/ampersand-api-openapi-original.yml
  type: apiKey
- bearerFormat: JWT
  name: Bearer
  scheme: bearer
  sources:
  - openapi/ampersand-api-openapi-original.yml
  type: http
slug: ampersand-authentication
source_filename: ampersand-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ampersand-api-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/ampersand-api-openapi-original.yml\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ampersand-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/authentication/ampersand-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
---
